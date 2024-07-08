---
layout: post
title: "Volcano Maungawhau"
date: "2009-08-20"
tags: [dataset, script]
published: true
image: false
author: Tom Hengl
---

Maunga Whau (Mt Eden) is one of about 50 volcanos in the Auckland volcanic field. This data set gives topographic information for Maunga Whau on a 10 m by 10 m grid. A matrix with 87 rows and 61 columns, rows corresponding to grid lines running east to west and columns to grid lines running south to north.

Perspective view - volcano  

![]({{site.baseurl}}/uploads/img/posts/Fig_maungawhau.jpg)
  

**Available layers:** 

\- volcano\_maungawhau.asc --- the 10 m DEM digitized from the topo map;

**Grid definition:** 

ncols: 61  
nrows: 87  
xllcorner: 2667400  
yllcorner: 6478700  
cellsize: 10 m

**proj4:**+init=epsg:27200

**Lineage:** 

Digitized from a topographic map by Ross Ihaka. These data should not be regarded as accurate.  

```
\> data(volcano)
>library(spatstat)
>LLC <- data.frame(E=174.761345, N=-36.879784)
>coordinates(LLC) <- ~E+N
>proj4string(LLC) <- CRS("+proj=longlat +datum=WGS84")
>LLC.NZGD49 <- spTransform(LLC, CRS("+init=epsg:27200"))
>volcano.r <- as.im(list(x=seq(from=2667405, length.out=61, by=10),
+     y=seq(from=6478705, length.out=87, by=10), 
+     z=t(volcano)\[61:1,\]))
>volcano.sp <- as(volcano.r, "SpatialGridDataFrame")
>proj4string(volcano.sp) <- CRS("+init=epsg:27200")
# str(volcano.sp)
# spplot(volcano.sp, at=seq(min(volcano.sp$v), max(volcano.sp$v),5),
+    col.regions=topo.colors(45))
>write.asciigrid(volcano.sp, "volcano\_maungawhau.asc", na.value=-1)
```

**Data owner:** LINZ  
**Location**:Volcano Maungawhau, Auckland, New Zealand  
36° 50' 50.586" S,174° 45' 56.646" E  
See map: [Google Maps](http://maps.google.com/?q=Volcano%2C+%2CMaungawhau)

**_Attachment:_**  
[volcano_maungawhau.zip]({{site.baseurl}}/uploads/datasets/volcano_maungawhau.zip)
