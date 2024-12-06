---
layout: post
title: "Best BiCubic Method to Compute the Planimetric Misregistration between Images with Sub-Pixel Accuracy: Application to Digital Elevation Models"
date: "2024-03-25"
tags: [story,interpolation,srtm,aster,alos,fabdem,nasadem,copdem,copernicus,publication,demix]
published: true
image: false
author: C.H. Grohmann
---

There is a new paper (open access) describing a novel method to estimate sub-pixel planimetric displacements between two DEMs:

Riazanoff, S.; Corseaux, A.; Albinet, C.; Strobl, P.A.; López-Vázquez, C.; Guth, P.L.; Tadono, T. Best BiCubic Method to Compute the Planimetric Misregistration between Images with Sub-Pixel Accuracy: Application to Digital Elevation Models. _ISPRS Int. J. Geo-Inf._ 13, 96. [https://doi.org/10.3390/ijgi13030096](https://doi.org/10.3390/ijgi13030096)  

<!--more-->


**Paper abstract:**  
 In recent decades, an important number of regional and global digital elevation models (DEMs) have been released publicly. As a consequence, researchers need to choose between several of these models to perform their studies and to use these DEMs as third-party data to compute derived products (e.g., for orthorectification). However, the comparison of DEMs is not trivial. For most quantitative comparisons, DEMs need to be expressed in the same coordinate reference system (CRS) and sampled over the same grid (i.e., be at the same ground sampling distance with the same pixel-is-area or pixel-is-point convention) with heights relative to the same vertical reference system (VRS). Thankfully, many open tools allow us to perform these transformations precisely and easily. Despite these rigorous transformations, local or global planimetric displacements may still be observed from one DEM to another. These displacements or disparities may lead to significant biases in comparisons of DEM elevations or derived products such as slope, aspect, or curvature. Therefore, before any comparison, the control of DEM planimetric accuracy is certainly a very important task to perform. This paper presents the disparity analysis method enhanced to achieve a sub-pixel accuracy by interpolating the linear regression coefficients computed within an exploration window. This new method is significantly faster than oversampling the input data because it uses the correlation coefficients that have already been computed in the disparity analysis. To demonstrate the robustness of this algorithm, artificial displacements have been introduced through bicubic interpolation in an 11 × 11 grid with a 0.1-pixel step in both directionsThis validation method has been applied in four approximately 10 km × 10 km DEMIX tiles showing different roughness (height distribution). Globally, this new sub-pixel accuracy method is robust. Artificial displacements have been retrieved with typical errors (eb) ranging from 12 to 20% of the pixel size (with the worst case in Croatia). These errors in displacement retrievals are not equally distributed in the 11 × 11 grid, and the overall error Eb depends on the roughness encountered in the different tiles. The second aim of this paper is to assess the impact of the bicubic parameter (slope of the weight function at a distance d = 1 of the interpolated point) on the accuracy of the displacement retrieval. By considering Eb as a quality indicator, tests have been performed in the four DEMIX tiles, making the bicubic parameter vary between −1.5 and 0.0 by a step of 0.1. For each DEMIX tile, the best bicubic (BBC) parameter b* is interpolated from the four Eb minimal values. This BBC parameter b* is low for flat areas (around −0.95) and higher in mountainous areas (around −0.75). The roughness indicator is the standard deviation of the slope norms computed from all the pixels of a tile. A logarithmic regression analysis performed between the roughness indicator and the BBC parameter b* computed in 67 DEMIX tiles shows a high correlation (r = 0.717). The logarithmic regression formula estimating the BBC parameter from the roughness indicator is generic and may be applied to estimate the displacements between two different DEMs. This formula may also be used to set up a future Adaptative Best BiCubic (ABBC) that will estimate the local roughness in a sliding window to compute a local BBC.



