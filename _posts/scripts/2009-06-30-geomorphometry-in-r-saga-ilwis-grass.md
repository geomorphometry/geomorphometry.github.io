---
layout: post
title: "Geomorphometry in R + SAGA + ILWIS + GRASS"
date: "2009-06-30"
tags: [dataset, script]
published: true
image: false
author: Tom Hengl
---

This is a sample [code]({{site.baseurl}}/uploads/datasets/SAGA_ILWIS_GRASS_0.zip) to process Baranja hill DEM using a combination of R, SAGA, ILWIS and Google Earth (under MS Windows machines). All four packages are available as open source or freeware (GE). You first need to obtain and install [**R**](http://www.r-project.org/) (including the maptools, gstat, rgdal and RSAGA packages), **[ILWIS 3.5](http://52north.org/index.php?option=com_content&task=view&id=219&Itemid=320)**, [**SAGA GIS**](http://www.saga-gis.org/) and [**GRASS GIS**](http://grass.osgeo.org/). After you finished [installing R, SAGA, ILWIS, GRASS](http://spatial-analyst.net/wiki/index.php?title=Software), copy the code down-below and start running it line by line. If you experience problems, send as a post via the **[R-sig-geo](https://stat.ethz.ch/mailman/listinfo/r-sig-geo)** or **[ILWIS mailing list](https://52north.org/mailman/listinfo/ilwis)**. Note: in order to use the functionality of ILWIS, SAGA, GRASS, you need to install them first. These are not internal packages in R!

 ![]({{site.baseurl}}/uploads/img/posts/R_GRASS_screen.jpg)

Fig: Screenshots of R + SAGA/GRASS/ILWIS integration

```
######## R script ###############
# DEM processing and extraction of channel networks;
library(maptools)
library(rgdal)
library(RSAGA)
# ! first download and install SAGA GIS [http://www.saga-gis.org], ILWIS GIS [https://52north.org/download/Ilwis/52n-Ilwis-v3-05-02.zip] and GRASS GIS [http://grass.itc.it] to your machine!
rsaga.env(path="C:/Progra~1/saga_vc")
ILWIS <- "C:\Progra~1\N52\Ilwis35\IlwisClient.exe -C"
MGI_Z6 <- "+proj=tmerc +lat_0=0 +lon_0=18 +k=0.9999 +x_0=6500000 +y_0=0 +ellps=bessel +towgs84=550.499,164.116,475.142,5.80967,2.07902,-11.62386,0.99999445824 +units=m"
# The coordinate system is "MGI Zone 6"; see [http://spatial-analyst.net/wiki/index.php?title=MGI_/_Balkans_coordinate_systems]
setwd("C:/tmp")
# obtain the data:
download.file("http://geomorphometry.org/system/files/BaranjaHill.zip", destfile=paste(getwd(), "BaranjaHill.zip", sep="/"))
fname <- zip.file.extract(file="DEM25m.asc", zipname="BaranjaHill.zip")
file.copy(fname, "./DEM25m.asc", overwrite=TRUE)
list.files(pattern="asc")
dem25m <- readGDAL("DEM25m.asc")
proj4string(dem25m) <- CRS(MGI_Z6)
# view the data in ILWIS:
writeGDAL(dem25m[1], "dem25m.mpr", "ILWIS")
# set the right coordinate system!
download.file("http://spatial-analyst.net/CRS/gk_6.csy", destfile=paste(getwd(), "gk_6.csy", sep="/"))
shell(cmd=paste(ILWIS, "setcsy dem25m.grf gk_6.csy -force"), wait=F)
shell(cmd=paste(ILWIS, "open dem25m.mpr -noask"), wait=F)
# make a relief view in ILWIS:
shell(cmd=paste(ILWIS, "run C:\Progra~1\Ilwis3\Scripts\Hydro-DEM\dem_visualization dem25m.mpr dem25m_c.mpr"), wait=F)
# load to SAGA and derive drainage network:
rsaga.esri.to.sgrd(in.grids="dem25m.asc", out.sgrds="dem25m.sgrd", in.path=getwd())
# First, fill the spurious sinks:
rsaga.get.modules("ta_preprocessor")
rsaga.get.usage("ta_preprocessor", 2)
rsaga.geoprocessor(lib="ta_preprocessor", module=2, param=list(DEM="dem25m.sgrd", RESULT="dem25m_f.sgrd", MINSLOPE=0.05))
# Second, extract the channel network:
rsaga.get.modules("ta_channels")
rsaga.get.usage("ta_channels", 0)
rsaga.geoprocessor(lib="ta_channels", module=0, param=list(ELEVATION="dem25m.sgrd", CHNLNTWRK="channel_ntwrk.sgrd", CHNLROUTE="channel_route.sgrd", SHAPES="channels2.shp", INIT_GRID="dem25m.sgrd", DIV_CELLS=3, MINLEN=40))
channels <- readOGR("channels.shp", "channels")
spplot(channels["LENGTH"], col.regions=bpy.colors())
# derive Topographic Wetness Index:
rsaga.geoprocessor(lib="ta_hydrology", module=15, param=list(DEM="dem25m.sgrd", C="catharea.sgrd", GN="catchslope.sgrd", CS="modcatharea.sgrd", SB="TWI.sgrd", T=10))
# Export of grids to Google Earth using SAGA GIS:
rsaga.geoprocessor(lib="pj_proj4", 2, param=list(SOURCE_PROJ=paste('"', proj4string(dem25m), '"', sep=""), TARGET_PROJ=""+proj=longlat +datum=WGS84"", SOURCE="TWI.sgrd", TARGET="TWI_ll.sgrd", TARGET_TYPE=0, INTERPOLATION=0))
# export to PNG:
rsaga.geoprocessor(lib="io_grid_image", 0, param=list(GRID="TWI_ll.sgrd", FILE="TWI.png"))
# read back to R:
rsaga.sgrd.to.esri(in.sgrds="TWI_ll.sgrd", out.grids="TWI_ll.asc", prec=1, out.path=getwd())
TWI.ll <- readGDAL("TWI_ll.asc")
proj4string(TWI.ll) <- CRS("+proj=longlat +datum=WGS84")
TWI.kml <- GE_SpatialGrid(TWI.ll)
kmlOverlay(TWI.kml, kmlfile="TWI.kml", imagefile="TWI.png", name="Topographic Wetness Index")
# Optional: export to Google Earth using ILWIS:
dem25m.ll <- spTransform(dem25m[1], CRS("+proj=longlat +datum=WGS84"))
corrf <- (1+cos((dem25m.ll@bbox[2,2]+dem25m.ll@bbox[2,1])/2*pi/180))/2
geogrd.cell <- corrf*(dem25m.ll@bbox[1,2]-dem25m.ll@bbox[1,1])/dem25m@grid@cells.dim[1]
geoarc <- spsample(dem25m.ll, type="regular", cellsize=c(geogrd.cell,geogrd.cell))
gridded(geoarc) <- TRUE
gridparameters(geoarc)
gridparameters(dem25m)
# resample the map (Bilinear) to the new geographic grid:
shell(cmd=paste(ILWIS, " crgrf geoarc.grf ",geoarc@grid@cells.dim[[2]]," ",geoarc@grid@cells.dim[[1]]," -crdsys=LatlonWGS84 -lowleft=(",geoarc@grid@cellcentre.offset[[1]],",",geoarc@grid@cellcentre.offset[[2]],") -pixsize=",geoarc@grid@cellsize[[1]],sep=""), wait=F)
shell(cmd=paste(ILWIS, "dem25m_ll_c.mpr = MapResample(dem25m_c.mpr, geoarc, BiLinear)"), wait=F)
shell(cmd=paste(ILWIS, "open dem25m_ll_c.mpr -noask"))
shell(cmd=paste(ILWIS, "export tiff(dem25m_ll_c.mpr, dem25m_c.tif)"), wait=F)
# generate a KML (ground overlay):
dem25m.kml <- GE_SpatialGrid(geoarc)
kmlOverlay(dem25m.kml, "dem25m_c.kml", "dem25m_c.tif", name="Shaded relief in ILWIS")
# export of extracted channels to Google Earth:
proj4string(channels) <- CRS(MGI_Z6)
channels.ll <- spTransform(channels[3], CRS("+proj=longlat +datum=WGS84"))
writeOGR(channels.ll, "channels.kml", "channels", "KML")
# extract the drainage network in GRASS GIS:
library(spgrass6) # version => 0.6-1 (http://spatial.nhh.no/R/Devel/spgrass6_0.6-1.zip (71))
# Location of your GRASS installation:
loc <- initGRASS("C:/GRASS", home=tempdir())
loc
# Import the ArcInfo ASCII file to GRASS:
parseGRASS("r.in.gdal") # commmand description
execGRASS("r.in.gdal", flags="o", parameters=list(input="DEM25m.asc", output="DEM"))
execGRASS("g.region", parameters=list(rast="DEM"))
gmeta6()
# extract the drainage network:
execGRASS("r.watershed", flags=c("m", "overwrite"), parameters=list(elevation="DEM", stream="stream", threshold=as.integer(50)))
# thin the raster map so it can be converted to vectors:
execGRASS("r.thin", parameters=list(input="stream", output="streamt"))
# convert to vectors:
execGRASS("r.to.vect", parameters=list(input="streamt", output="streamt", feature="line"))
streamt <- readVECT6("streamt")
plot(streamt)
######## R script ###############
```		

MORE READING:

1. Bivand, R. 2005. [**Interfacing GRASS 6 and R. Status and development directions**](http://grass.itc.it/newsletter/GRASSNews_vol3.pdf), GRASS Newsletter, 3, 11–16.
2. Bivand, R., Pebesma, E., Rubio, V., 2008. [**Applied Spatial Data Analysis with R**](http://www.asdar-book.org/). Use R Series, p. 400. Springer, Heidelberg, pp. 378.
3. Brenning, A. 2008. [**Statistical geocomputing combining R and SAGA: The example of landslide susceptibility analysis with generalized additive models**](http://www.environment.uwaterloo.ca/u/brenning/Brenning-2008-RSAGA.pdf). In: J. Böhner, T. Blaschke & L. Montanarella (eds.), SAGA - Seconds Out (= Hamburger Beiträge zur Physischen Geographie und Landschaftsökologie, 19), 23-32.
4. Conrad, O. 2007. [**SAGA — Entwurf, Funktionsumfang und Anwendung eines Systems fur Automatisierte Geowissenschaftliche Analysen**](http://www.saga-gis.org/en/about/references.html), Ph.D. thesis, University of Gottingen, Gottingen.
5. Grohmann, C.H. 2004. [**Morphometric analysis in Geographic Information Systems: applications of free software GRASS and R**](http://dx.doi.org/10.1016/j.cageo.2004.08.002). Computers & Geosciences, 30 (9-10):1055-1067.
6. Hengl, T., 2009. [**A Practical Guide to Geostatistical Mapping**](http://spatial-analyst.net/book/). 2nd Ed, University of Amsterdam, 291 p.
7. Neteler, M. and Mitasova, H. 2008. [**Open Source GIS: A GRASS GIS Approach**](http://www.grassbook.org/), Springer, New York, 3rd edn.

_**Attachment:**_

[SAGA\_ILWIS\_GRASS\_0.zip]({{site.baseurl}}/uploads/datasets/SAGA_ILWIS_GRASS_0.zip)



