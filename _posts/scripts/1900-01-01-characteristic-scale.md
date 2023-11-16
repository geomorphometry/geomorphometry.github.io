---
layout: post
title: "Characteristic scale"
date: "2009-08-21"
tags: [dataset, script]
published: true
image: false
author: J. Wood
---

**Short title**:  characteristicScale.lsc

Inputs: A DEM (the Baranja Hill 25m DEM is used as an example). The name of the parameter to measure and the minimum and maximum window sizes over which to measure it.  
Outputs: Two rasters, one containing the measured parameter, the other the window size at which the parameter is most extreme.

**Purpose and use**: 

Finds the scale at which a geomorphometric parameter is most extreme for each cell in a DEM. Part of this script appears in Hengl and Reuter (2008) \[the Geomorphometry book\].  
Script to measure surface parameter at characteristic scales. It is designed to incorporate scale-based analysis into surface parameterisation. It measures the given parameter (e.g. slope, profile curvature etc.) at a range of scales, and finds the scale at which that parameter is most extreme. Can be used to explore scale sensitivity of a surface.

**Programming environment**:  Landserf  
**Status of work**:  Public Domain  
**Reference**:  [Geomorphometry: Concepts, Software, Applications](https://books.google.com.gi/books?id=u33ArNw4BacC&printsec=frontcover&source=gbs_book_other_versions_r&cad=4#v=onepage&q&f=false)  
**Data set name**:  [Baranja hill]({{site.baseurl}}/2020/06/30/baranja-hill)

* * *

**_Attachment:_**

[characteristicScale.lsc_.zip]({{site.baseurl}}/uploads/datasets/characteristicScale.lsc_.zip)
