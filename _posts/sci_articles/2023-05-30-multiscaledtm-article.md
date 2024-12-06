---
layout: post
title: "MultiscaleDTM: An open-source R package for multiscale geomorphometric analysis"
date: "2023-05-3"
tags: [story,publication,toolbox,r,cran,package]
published: true
image: false
author: C.H. Grohmann
---

There is a new paper (open access) describing an R package for multiscale geomorphometric analysis:

Ilich, A.R., Misiuk, B., Lecours, V., Murawski, S.A. 2023. MultiscaleDTM: An open-source R package for multiscale geomorphometric analysis. Transactions in GIS, 27, 1164–1204. [https://doi.org/10.1111/tgis.13067](https://doi.org/10.1111/tgis.13067)

<!--more-->


**Paper abstract:**  
Digital terrain models (DTMs) are datasets containing altitude values above or below a reference level, such as a reference ellipsoid or a tidal datum over geographic space, often in the form of a regularly gridded raster. They can be used to calculate terrain attributes that describe the shape and characteristics of topographic surfaces. Calculating these terrain attributes often requires multiple software packages that can be expensive and specialized. We have created a free, open-source R package, MultiscaleDTM, that allows for the calculation of members from each of the five major thematic groups of terrain attributes: slope, aspect, curvature, relative position, and roughness, from a regularly gridded DTM. Furthermore, these attributes can be calculated at multiple spatial scales of analysis, a key feature that is missing from many other packages. Here, we demonstrate the functionality of the package and provide a simulation exploring the relationship between slope and roughness. When roughness measures do not account for slope, these attributes exhibit a strong positive correlation. To minimize this correlation, we propose a new roughness measure called adjusted standard deviation. In most scenarios tested, this measure produced the lowest rank correlation with slope out of all the roughness measures tested. Lastly, the simulation shows that some existing roughness measures from the literature that are supposed to be independent of slope can actually exhibit a strong inverse relationship with the slope in some cases.






