---
layout: post
title: "North Carolina coast LiDAR"
date: "2011-10-09"
tags: [dataset, script]
published: true
image: false
author: Tom Hengl
---

This dataset contains a series of x,y,z LiDAR point cloud data in csv format, delimited by comma. Points are projected in the NC State Plane [EPSG 3358](http://spatialreference.org/ref/epsg/3358/) coordinate system with units meters.

To get more better representation of structures from LiDAR surveys,  
re-interpolate to 0.3-0.5m resolution using the available external point clouds [nc\_coast\_pointseries.zip]({{site.baseurl}}/uploads/datasets/nc_coast_demseries.zip).

**Available layers:** 

- "JR\_NED\_\*" - 1/3 and 1/9-Arc Second National Elevation Dataset (2 m);
- "ortho\_JR\_\*" - Time series of ortho photos (1932, 1945, 1955, 1974, 1988, 1998, 2007, 2009);
- "JR\_\*.csv" - Time series of point clouds from LiDAR (1974, 1995, 1996, 1997, 1998, 1999, 2001, 2005, 2007, 2008, 2009)

**Grid definition:** 

  min  max  
x 912884 914112  
y 250049 250905

cellsize: 2 m  
cells.dim: 614 by 428

**proj4**: +proj=lcc +lat\_1=36.16666666666666 +lat\_2=34.33333333333334 +lat\_0=33.75 +lon\_0=-79 +x\_0=609601.22 +y\_0=0 +ellps=GRS80 +units=m +no\_defs

**Lineage:** 

All other data sets are from lidar, but the coverage varies, some data sets cover only beach and foredune area and do not include the main dune. Date of the surveys is in the name of of the file in the form YYYY\_MM\_DD.

**Data owner**: USGS / NCSU  
**Reference**: [Landscape dynamics from LiDAR data time series]({{site.baseurl}}/uploads/pdf/pdf2011/Mitasova2011geomorphometry.pdf)  
**Location**: NC, United States  
35° 57' 41.148" N, 75° 37' 49.152" W  
See map: [Google Maps](http://maps.google.com/?q=35.961430+-75.630320+%2C+us)

* * *

**_Attachment:_**

[nc\_coast\_pointseries.zip]({{site.baseurl}}/uploads/datasets/nc_coast_demseries.zip)

[JR\_maps]({{site.baseurl}}/uploads/datasets/JR_maps.zip)

[JR\_2009\_11\_27]({{site.baseurl}}/uploads/datasets/JR_2009_11_27.7z)

[JR\_2008\_03\_27]({{site.baseurl}}/uploads/datasets/JR_2008_03_27.7z)

[JR\_2007\_07\_08]({{site.baseurl}}/uploads/datasets/JR_2007_07_08.7z)

[JR\_2005\_11\_26]({{site.baseurl}}/uploads/datasets/JR_2005_11_26.7z)

[JR\_2004\_09\_25]({{site.baseurl}}/uploads/datasets/JR_2004_09_25.7z)

[JR\_2001\_02\_15]({{site.baseurl}}/uploads/datasets/JR_2001_02_15.7z)

[JR\_1999\_11\_04]({{site.baseurl}}/uploads/datasets/JR_1999_11_04.7z)

[JR\_1999\_09\_18]({{site.baseurl}}/uploads/datasets/JR_1999_09_18.7z)

[JR\_1999\_09\_09]({{site.baseurl}}/uploads/datasets/JR_1999_09_09.7z)

[JR\_1998\_07\_01]({{site.baseurl}}/uploads/datasets/JR_1998_07_01.7z)

[JR\_1997\_10\_02]({{site.baseurl}}/uploads/datasets/JR_1997_10_02.7z)

[JR\_1996\_10\_16]({{site.baseurl}}/uploads/datasets/JR_1996_10_16.7z)

[JR\_1995\_07\_01]({{site.baseurl}}/uploads/datasets/JR_1995_07_01.7z)

[JR\_1974\_07\_01]({{site.baseurl}}/uploads/datasets/JR_1974_07_01.7z)
