---
layout: post
title: "Baranja hill"
date: "2009-08-17"
tags: [dataset, script]
published: true
image: false
author: Tom Hengl
---

The Baranja Hill study area, located in eastern Croatia, has been mapped extensively over the years and several GIS layers are available at various scales. Its main geomorphic features include hill summits and shoulders, eroded slopes of small valleys, valley bottoms, a large abandoned river channel, and river terraces. All raster images are prepared in the ArcInfo ASCI grid format. The vector maps are prepared as shape files. In addition to the GIS layers, you might also need to use the field observations. Courtesy of the [Croatian State Geodetic Department](http://www.dgu.hr/).

Fig: preview of the main GIS layers

- ![]({{site.baseurl}}/uploads/img/data/data_topo5K.jpg)    Topomap 1:5K  
    
- ![]({{site.baseurl}}/uploads/img/data/data_DEM25m.jpg)    25m DEM  
    
- ![]({{site.baseurl}}/uploads/img/data/data_geoforms.jpg)  Geoforms  
    
- ![]({{site.baseurl}}/uploads/img/data/data_landcover.jpg) Landcover  
    
- ![]({{site.baseurl}}/uploads/img/data/data_ortho.jpg)     Orthophoto  
    
- ![]({{site.baseurl}}/uploads/img/data/data_satimage.jpg)  Landsat  
    
- ![]({{site.baseurl}}/uploads/img/data/data_contours5K.jpg) Contours  
    
- ![]({{site.baseurl}}/uploads/img/data/data_DEM5m.jpg)  25m SRTM  
    



This data set has been used extensively in the Geomorphometry book:

Hengl, T., Reuter, H.I. (eds) 2008.**Geomorphometry: Concepts, Software, Applications**. Developments in Soil Science, vol. 33, Elsevier, 772 pp. ISBN: 978-0-12-374345-9  


Available layers:

\- DEM25m - 25 m resolution DEM derived from the 1:5K contours (ArcInfo ASCI grid format);  
\- contours.shp - Contour lines digitized from the 1:50K topo maps (ESRI Shapefile);  
\- contours5K.shp - Contour lines digitized from the 1:5K topo maps (ESRI Shapefile);  
\- wstreams.shp - Streams and water bodies digitized from the 1:50K topo maps (ESRI Shapefile);  
\- elevations.shp - very precise elevation measurements from 1:5K land survey (ESRI Shapefile);  
\- DEM25srtm.asc - 25 m resolution DEM from SRTM 2000 project ordered via [http://eoweb.dlr.de](http://eoweb.dlr.de/) (ArcInfo ASCI grid format);  
\- orthophoto.tif - 5 m resolution ortophoto (ArcInfo ASCI grid format);  
\- topo5K.tif - Topo map 1:5000 (geotif, 23 MB);  
\- satimage.lan - 25 m resolution Landsat 7 image from September 1999 (ERDAS .lan format);  
\- landcover.shp - Land cover map digitized from the ortophoto (ESRI Shapefile);  
\- geoform.shp - Map of the geoforms using the geopedological approach (ESRI Shapefile);Grid definition:

ncols: 147  
nrows: 149  
xllcorner: 6551884  
yllcorner: 5070562  
cellsize: 25 mproj4:+proj=tmerc +lat\_0=0 +lon\_0=18 +k=0.9999 +x\_0=6500000 +y\_0=0 +ellps=bessel +towgs84=550.499,164.116,475.142,5.80967,2.07902,-11.62386,0.99999445824 +units=mLineage:

50K and 5K scale topomaps and aerial photo have been obtained from the Croatian State Geodetic Department ([http://www.dgu.hr](http://www.dgu.hr/)). Orthorectified photo was produced following the methodology explained in Rossiter & Hengl (2002). From the orthophoto we digitized on-screen land cover polygon map using the following classes: agricultural fields, fish ponds, natural forest, pasture and grassland, and urban areas. From the stereo-pairs we interpreted the generic landforms and then created a polygon map of geoforms (see also Rossiter & Hengl (2002)). Nine landform elements were recognised: summit, hill shoulder, escarpment, colluvium, hillslope, valley bottom, glacis (sloping), high terrace (tread) and low terrace (tread). From topomaps, we extracted contours and streams and water bodies. In the case of 1:50K the equidistance was 20 m in hilland and 5 m in plain, and for the 1:5K the equidistance was 5 m in hilland and 1 m in plain. From the 1:5K contours and geodetic points, the 5 m DEM has been derived using the ANUDEM (topogrid) procedure in ArcInfo and then resampled to the 25 m gird. The 30 m SRTM DEM (15'x15' block) was ordered from the German Aerospace Agency ([http://eoweb.dlr.de](http://eoweb.dlr.de/)), then resampled to the 25 grid so it can be compared with the DEM25m. IMPORTANT NOTE: According to a licence agreement, the SRTM dataset can not be distributed or used for commercial purposes outside this project.

**Data owner:** Croatian State Geodetic Department  
**Reference:** [Technical note: Creating geometrically-correct photo-interpretations, photomosaics, and base maps for a project GIS (PDF)](https://www.css.cornell.edu/faculty/dgr2/_static/files/pdf/TN_Georef_wFigs_Screen_v3.pdf)  

**Location:** Baranja hill, Popovac, Croatia  
45° 48' 16.4412" N, 18° 39' 54.198" E
See map: [Google Maps](https://maps.app.goo.gl/nW1EQK3m4QZhyTDD9)
* * *

**_Attachment:_**

[baranjahill.R]({{site.baseurl}}/uploads/datasets/baranjahill.R)

[BaranjaHill.zip]({{site.baseurl}}/uploads/datasets/BaranjaHill.zip)

[BaranjaHill_photo.zip]({{site.baseurl}}/uploads/datasets/BaranjaHill_photo.zip)

[BaranjaHill_topo5k.zip]({{site.baseurl}}/uploads/datasets/BaranjaHill_topo5k.zip)
