---
layout: post
title: "Ebergotzen"
date: "2009-08-20"
tags: [dataset, script]
published: true
image: false
author: Tom Hengl
---

Ebergötzen is 10x10 km study area in the vicinity of the city of Göttingen in Central Germany (51°30'03.16''--51°35'31.45''N; 10°00'28.67''--10°09'15.21''E). This area has been extensively surveyed over the years, mainly for the purposes of developing operational digital soil mapping techniques. The dataset has also been frequently used by the [SAGA development team](http://www.saga-gis.org/) and the [SciLands GmbH](http://www.scilands.de/) in many of their demonstrations and documents.

Courtesy of [Gehrt Ernst](mailto:Ernst.Gehrt@niedersachsen.de), the State Authority for Mining, Energy and Geology, Hannover, Germany.

The final Google Earth layout showing predicted soil texture fractions in topsoil.  
![]({{site.baseurl}}/uploads/img/data/Fig_ebergotzen.jpg)

**Available layers:** 

\- points.dbf - the point dataset consists of lab measurements four variables are available: SAND, SILT and CLAY (all expressed as % of mass measured for the 0-30 cm layer of soil) and SOILTYPE (type of soil based on the German classification system).  
\- DEM25.asc - 25 m DEM derived from the topo-maps;  
\- DEM100.asc - 100 m SRTMDEM;  
\- landimg.lan - LANDSAT image bands obtained from the http://image2000.jrc.it Corine Land Cover 2000 Project. The image consists of seven bands.  
\- ZONES.asc - 1:50.000 geological map of Germany.

**Grid definition:** 

ncols: 400  
nrows: 400  
xllcorner: 3570000  
yllcorner: 5708000  
cellsize: 25 mproj4:+init=epsg:31467

**Lineage:**
All input raster maps are in ArcInfo \*.asc format, and the point data (tables) are in a \*.dbf format. All coordinates are in the official German coordinate system, zone 3 (germany3): Transverse Mercator Projection, central meridian is 9°, false easting 3500000, Bessel 1841 ellipsoid with Potsdam datum. The bounding coordinates of the study area are: XMIN=3570000, YMIN=5708000, XMAX=3580000, YMAX=5718000. The input raster maps are available in two grid resolutions: 25 m (fine) and 100 m (coarse). The sand, silt and clay values have been determined by using the so-called_texture by hand_method: a surveyor distinguishes to which of the 32 texture classes a soil samples belongs to, and then estimates the content of fractions. E.g. texture class**St2**has 10% clay, 25% silt and 65% sand.

**Data owner**: State Authority for Mining, Energy and Geology, Hannover, Germany  
**Reference**: Gehrt, E., Buhner, J., (2001) Vom punkt zur flache — probleme des 'upscaling' in der bodenkartierung. In: Diskussionsforum Bodenwissenschaften: Vom Bohrstock zum Bildschirm. FH, Osnabruck, pp. 17-34. 

**Location**:Ebergotzen, Germany  
51° 34' 19.2324" N,10° 6' 28.7964" E  
See map:[Google Maps](http://maps.google.com/?q=Ebergotzen%2C+de)

* * *

**_Attachment:_**

[ebergotzen.zip]({{site.baseurl}}/uploads/datasets/ebergotzen.zip)

[ebergotzen_input.zip]({{site.baseurl}}/uploads/datasets/ebergotzen_input.zip)
