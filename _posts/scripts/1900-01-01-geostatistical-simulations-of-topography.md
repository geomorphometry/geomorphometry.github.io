---
layout: post
title: "Geostatistical simulations of topography"
date: "2009-08-20"
tags: [dataset, script]
published: true
image: false
author: Tom Hengl
---

**Short title**:  DEMsim

Inputs: control.txt - 1020 precise measurements (photogrametric + spot heights); elevations.txt - 2051 points (contours + spot heights); dem10m\_tin.asc - 100x150 pixels 30m DEM.  
Outputs: simulated DEMs, simulated error surfaces, error assessment statistics.

**Purpose and use:** 

Script to generate and simulate DEMs and assess the error of the height measurements. Prepared for the needs of a research paper 'Geostatistical modelling of topography using auxiliary maps'. Please consider testing the script before you use it with large datasets.

**Programming environment**:  R / S language  
**Status of work:**  Public Domain  
**Reference:**  [{Geostatistical modelling of topography using auxiliary maps}](https://doi.org/10.1016/j.cageo.2008.01.005)  
**Data set name:** [Zlatibor]({{site.baseurl}}/2020/06/30/zlatibor/)

**_Attachment:_**

[zlatibor-1.zip]({{site.baseurl}}/uploads/datasets/zlatibor-1.zip)





