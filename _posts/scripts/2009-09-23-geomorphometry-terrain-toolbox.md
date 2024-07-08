---
layout: post
title: "geomorphometry terrain toolbox"
date: "2009-09-23"
tags: [dataset, script]
published: true
image: false
author: Hannes Reuter
---

Short title:  amltools

ArcInfo Arc Marco Language Code (AML) Geomorphometry Toolbox contains a collection of terrain analysis scripts which can be used with a installation of ArcInfo's Workstation. Please note: They are not working with ARCVIEW and also not directly with ArcGIS, even if it is possible to run AML Code from inside ArcGIS. Still, you need ArcInfo Work Station installed. For a quick start please refer to readme.txt for some command calls or to the outdated topomanual2.pdf.

The ArcGIS Geomorphomerty Python toolbox (DEMO Version) works  up to a cell limit of 5000 cells. It contains a significant larger amount of functionality. As of Version 1.0.6 you do not need ArcInfo WS to be installed anymore if AG10 is installed. I rewrote IFTHENELSE and DOCELL in python. Previous Versions(AG9.4) will still need to install ArcInfo Workstation on your machine as ESRI programmers have not been able to port certain GRID functions as DOCELL. The gtb\_demo zip contains now three different zip files for the respective Python Version (2.4-2.6) you might be using. If you get the magic number error, the installed tollbox does not match your installed python version. Current Version is 1.0.6.

For further information and FULL version please refer to [www.ai-relief.org](http://www.ai-relief.org/).

**Programming environment**:  Arc AML  
**Status of work**:  Public Domain  
**Reference**:  [Geomorphometry: Concepts, Software, Applications](https://books.google.com.gi/books?id=u33ArNw4BacC&printsec=frontcover&source=gbs_book_other_versions_r&cad=4#v=onepage&q&f=false)

[geomorphometry_aml.zip]({{site.baseurl}}/uploads/datasets/geomorphometry_aml.zip)

[gtb_demoV1.0.6_0.zip]({{site.baseurl}}/uploads/datasets/gtb_demoV1.0.6_0.zip)
