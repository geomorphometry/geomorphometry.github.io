---
layout: post
title: "Transformation (normalization) tool"
date: "2015-01-19"
tags: [dataset, script]
published: true
image: false
author: Tom Hengl
---

Short title:  transform

**_Inputs:_** Slope raster or curvature raster; any other variables with skewed or long-tailed distributions  
_**Outputs:**_ Normalized slope or curvature raster; a text file informing about transformation used and new skewness/kurtosis.

For **INSTRUCTIONS**, please visit: [http://research.enjoymaps.ro/downloads/](http://research.enjoymaps.ro/downloads/)

**Reference:**  
[Csillik, O., Evans, I.S., Drăguţ, L., 2015. Transformation (normalization) of slope gradient and surface curvatures, automated for statistical analyses from DEMs. Geomorphology **232**(0): 65-77.](http://www.sciencedirect.com/science/article/pii/S0169555X15000033#)  

Purpose and use: 

Automated procedures are developed to alleviate long tails in frequency distributions of morphometric variables. They minimize the skewness of slope gradient frequency distributions, and modify the kurtosis of profile and plan curvature distributions towards that of the Gaussian (normal) model. Box-Cox (for slope) and arctangent (for curvature) transformations are used. The transforms are applicable to morphometric variables and many others with skewed or long-tailed distributions. It is suggested that such transformations should be routinely applied in all parametric analyses of long-tailed variables. Our Box-Cox and curvature automated transformations are based on a Python script, implemented as an easy-to-use script tool in ArcGIS.

**Programming environment:**  Python  
**Status of work:**  Public Domain

[Transformation-Tools.zip]({{site.baseurl}}/uploads/datasets/Transformation-Tools.zip)
