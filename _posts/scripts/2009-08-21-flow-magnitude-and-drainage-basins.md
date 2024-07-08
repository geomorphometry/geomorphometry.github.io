---
layout: post
title: "Flow magnitude and drainage basins"
date: "2009-08-21"
tags: [dataset, script]
published: true
image: false
author: J. Wood
---

**Short title:**flowMag.lsc

Inputs:A DEM (the Baranja Hill 25m DEM is used as an example).  
Outputs:A raster containing flow magnitude values for the DEM and a raster containing drainage basins.

**Purpose and use:** 

Script to calculate flow magnitude and drainage basins from a DEM. It demonstrates how recursive function calls in LandScript can be used to calculate zonal geomorphometric parameters using map algebra. To use this script, start LandSerf 2.3 or above and then open the LandScript editor (menu: Edit->LandSctipt Editor).  
Part of this script appears in Chapter 14 of Hengl and Reuter (2008) \[the Geomorphometry book\]. This script runs slowly so is better as a demonstration of how recursive function calls can be made in LandScript rather than a production quality flow magnitude calculator.

**Programming environment**:Landserf  
**Status of work**:Public Domain  
**Reference**:  [Geomorphometry: Concepts, Software, Applications](https://books.google.com.gi/books?id=u33ArNw4BacC&printsec=frontcover&source=gbs_book_other_versions_r&cad=4#v=onepage&q&f=false)  
**Data set name**:  [Baranja hill]({{site.baseurl}}/2020/06/30/baranja-hill)

**_Attachment:_**

[flowMag.lsc_.zip]({{site.baseurl}}/uploads/datasets/flowMag.lsc_.zip)





