---
layout: post
title: "Workshop: Automated analysis of elevation data in R+SAGA/GRASS"
date: "2009-08-25"
tags: [story,event,Zurich,Switzerland,workshop]
published: true
image: false
---

**Workshop moderators:**

1. [Tomislav Hengl](http://home.medewerker.uva.nl/t.hengl/) (University of Amsterdam)
2. [Carlos H. Grohmann](http://www.carlosgrohmann.com) (University of Sao Paulo)

**Location**: [Room 25H86/92]({{site.baseurl}}/uploads/pdf/pdf2009/map_of_events.pdf). This is a double room with a divider. Access will be through a locked door.

**Internet:** YES (Ethernet)

Please let us know about your impression of SAGA/GRASS by filling out this **web-form**.

Literature: 

- Chapters 8 and 9 in: Hengl, T. 2009. [**A Practical Guide to Geostatistical Mapping of Environmental Variables**](http://spatial-analyst.net/book/). EUR 22904 EN, Luxembourg: Office for Official Publications of the European Communities, 264 p.
- Conrad, O. 2007. [**SAGA — Entwurf, Funktionsumfang und Anwendung eines Systems fur Automatisierte Geowissenschaftliche Analysen**](http://www.saga-gis.org/en/about/references.html), Ph.D. thesis, University of Gottingen, Gottingen.
- Grohmann, C.H., Steiner, S.S., 2008. [SRTM resample with Short Distance-Low Nugget Kriging](http://dx.doi.org/10.1080/13658810701730152). International Journal of Geographical Information Science, 22 (8):895-906.
- Grohmann, C.H., 2008. [Introdução à Análise Digital de Terreno com GRASS-GIS](http://www.igc.usp.br/pessoais/guano/downloads/tutorial_grass6.pdf). Institute of Geosciences, University of São Paulo.
- Neteler, M. and Mitasova, H. 2008. **[Open Source GIS: A GRASS GIS Approach](http://www.grassbook.org/)**, Springer, New York, 3rd edn.

![]({{site.baseurl}}/uploads/img/meet2009/P8290006.JPG)

Fig: Room 25H86/92

**Daily programme:**

* * *

DAY 1 29.08.2009

<table border="0" width="90%" cellspacing="2" cellpadding="2"><tbody><tr><td width="85">0900-1030</td><td><p>Introduction to the workshop<br>Introduction to SAGA/GRASS; history and main functionality; the role of open source software; (T. Hengl, C.H. Grohmman)</p></td></tr><tr bgcolor="#666666"><td width="85">1030-1100</td><td>Coffee break</td></tr><tr><td width="85">1100-1300</td><td>Installation of necessary packages (R, SAGA, GRASS, Google Earth)</td></tr><tr><td width="85">&nbsp;</td><td>Introduction to the case study: “Fishcamp”</td></tr><tr><td width="85">&nbsp;</td><td>Computer exercises in SAGA: loading data, running SAGA commands from R and scripting, interpretation of results (T. Hengl, C.H. Grohmman)</td></tr><tr bgcolor="#666666"><td width="85">1300-1400</td><td>Lunch</td></tr><tr><td width="85">1400-1600</td><td>Computer exercises (individual)</td></tr><tr bgcolor="#666666"><td width="85">1545-1615</td><td>Coffee break</td></tr><tr><td width="85">1615-1730</td><td>Solving computer exercises (with assistance)</td></tr><tr><td width="85">&nbsp;</td><td>Q &amp; A’s / final discussion (T. Hengl)</td></tr><tr bgcolor="#666666"><td width="85">2030-23:00</td><td>Dinner at the campus (optional)</td></tr></tbody></table>

* * *

DAY 2 30.08.2009

<table border="0" width="90%" cellspacing="2" cellpadding="2"><tbody><tr><td width="85">0930-1030</td><td><p>Introduction to GRASS GIS: main functionality and operations; GRASS syntax (C.H. Grohmman)</p></td></tr><tr bgcolor="#666666"><td width="85">1030-1100</td><td>Coffee break</td></tr><tr><td width="85">1100-1300</td><td><p>Computer exercises in GRASS: loading data, running GRASS commands from R and scripting, interpretation of results (demonstration)</p></td></tr><tr><td width="85">&nbsp;</td><td>(C.H. Grohmman, T. Hengl)</td></tr><tr bgcolor="#666666"><td width="85">1300-1400</td><td>Lunch</td></tr><tr><td width="85">1400-1530</td><td>Computer exercises (individual)</td></tr><tr bgcolor="#666666"><td width="85">1530-1545</td><td>Coffee break</td></tr><tr><td width="85">1615-1730</td><td>Solving computer exercises (C.H. Grohmman)</td></tr><tr><td width="85">&nbsp;</td><td><a href="http://geomorphometry.org/content/saga-vs-grass-users-satisfaction">Q &amp; A’s / SAGA verus GRASS questionairre</a>&nbsp;(T. Hengl)</td></tr><tr bgcolor="#666666"><td width="85">2000-late</td><td>Dinner in the city (optional)</td></tr></tbody></table>

**Late registrations**: 15th of August; after that no more registrations are possible;

![]({{site.baseurl}}/uploads/img/logos/workshop_logo.jpg)

**Description:** This workshop aims at PhD students and professionals interested to use open source software packages for processing of their elevation data. R is the open-source version of the S language for statistical computing; SAGA (System for Automated Geoscientific Analyses) and GRASS (Geographic Resources Analysis Support System) are the two most used open-source desktop GIS for automated analysis of elevation data. A combination of R+SAGA/GRASS provides a full integration of statistics and geomorphometry. The topics in this workshop will range from selection of grid cell size, choice of algorithms for DEM generation and filtering, to geostatistical simulations and error propagation. The workshop moderators will demonstrate that R+SAGA/GRASS is capable of handling such demanding tasks as DEM generation from auxiliary maps, automated classification of landforms, and sub-grid parameterization of surface models.

The course will focus on understanding R and SAGA/GRASS syntax and building scripts that can be used to automate DEM-data processing. Each participant should come with a laptop PC and install all software needed prior to the workshop. Registered participants will receive an USB stick with all data sets and overheads at the beginning of the course.  
Participants will follow a case study that focuses on generation of DEMs, extraction of DEM parameters and landform classes, and implementation of error propagation in geomorphometry.

* * *

**SOFTWARE INSTALLATION**:

Please make sure you come to this workshop with software already installed and running. You need to install at least (please respect the chronological order):

1. **[R (2.9)](http://cran.r-project.org/bin/)**
    - after the installation open R and install necessary packages (install.views("Spatial"))
    - install separately packages "spgrass6" and "RSAGA"
2. **[Tinn-R](http://sourceforge.net/projects/tinn-r)**
3. **[GRASS GIS](http://grass.osgeo.org/grass64/binary/mswindows/) (6.4)**
4. SAGA GIS (2.0.3)
    - the latest version of SAGA will be distributed at the beginning of the workshop!

For simplicity, try to come with a Windows OS, possibly with a dual boot (Linux or Mac OS as the 2nd OS).  
Here are some [**examples of code**](https://geomorphometry.org/geomorphometry-in-r-saga-ilwis-grass/) that you could test under your machine.
