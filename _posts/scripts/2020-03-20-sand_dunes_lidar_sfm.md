---
layout: post
title: "Aeolian dune modelling with LiDAR and SfM-MVS"
date: "2020-03-20"
tags: [dataset, script, dune, sfm, lidar, grass, whitebox]
hide_hero: false
published: true
image: false
author: C.H. Grohmann
---

Github repository containing scripts and associated supplemental material (csv files, etc) for the paper:  

Grohmann,C.H.; Garcia,G.P.B.,; Affonso,A.A; Albuquerque,R.W., 2020. Dune migration and volume change from airborne LiDAR, terrestrial LiDAR and Structure from Motion-Multi View Stereo. _Computers & Geosciences_, 143:104569.  
View article at publisher (paywalled): [http://doi.org/10.1016/j.cageo.2020.104569](http://doi.org/10.1016/j.cageo.2020.104569)  
Open Access preprint (same content as article, different formatting): [https://arxiv.org/abs/1910.06186](https://arxiv.org/abs/1910.06186)  

**Link to GitHub repository:** [https://github.com/CarlosGrohmann/scripts_papers/tree/master/garopaba_als_sfm_tls](https://github.com/CarlosGrohmann/scripts_papers/tree/master/garopaba_als_sfm_tls)  


This paper presents an evaluation of Structure from Motion-Multi View Stereo (SfM-MVS) to obtain high-resolution elevation data of coastal sand dunes based on images acquired by Remotely Piloted Aircraft (RPA).  

The analyzes were made using [GRASS-GIS](https://grass.osgeo.org/) trough python scripts. Denoising of SfM-MVS DEMs were made with [WhiteBox](https://www.whiteboxgeo.com/). Although the DEMs cannot be shared in GitHub (due to space limitations), the scripts can be used as an educational resource.  

The LiDAR and SfM-MVS datasets can be accessed at:

- Airborne LiDAR 2010 - available at OpenTopography: [https://doi.org/10.5069/G9DN430Z](https://doi.org/10.5069/G9DN430Z)
- Terrestrial LiDAR 2019 - available at OpenTopography: [https://doi.org/10.5069/G9CN7228](https://doi.org/10.5069/G9CN7228)
- SfM-MVS 2019 - available at OpenTopography: [https://doi.org/10.5069/G9DV1H19](https://doi.org/10.5069/G9DV1H19)
- RPA images 2019 - available at GeoNadir: [https://data.geonadir.com/image-collection-details/334](https://data.geonadir.com/image-collection-details/334)

![]({{site.baseurl}}/uploads/img/posts/fig7_grohmann2020_garopaba.png)
Difference between LiDAR DEM (2010) and SfM-MVS DEM (2019) for the Garopaba dune field, in southern Brazil  

This study was supported by the Sao Paulo Research Foundation (FAPESP), Brazil grants #2009/17675-5 and #2016/06628-0 and by Brazil’s National Council of Scientific and Technological Development, CNPq grants #423481/2018-5 and #304413/2018-6 to C.H.G.  





