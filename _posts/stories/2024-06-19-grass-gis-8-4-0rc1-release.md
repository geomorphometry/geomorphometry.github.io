---
layout: post
title: "GRASS GIS 8.4.0RC1 release"
date: "2024-06-19"
tags: [story,software,foss,grass]
published: true
image: false
author: C.H. Grohmann
---

The GRASS GIS 8.4.0RC1 release provides more than 515 improvements and fixes with respect to the release 8.3.2.  

Check the full announcement at [https://github.com/OSGeo/grass/releases/tag/8.4.0RC1](https://github.com/OSGeo/grass/releases/tag/8.4.0RC1).  

Please support in testing this release candidate.  

<!--more-->

**Highlights**  
- *location* becomes *project*: The Python API, command line, and
graphical user interface are now using *project* instead of *location*
for the main component of the data hiearchy while maintaining backward
compatibility.
- v.fill.holes: New tool to remove inner isles and to keep outer
boundary only
- i.svm: New support vector machine image classification (SVM)
- r.horizon: Output for multiple points, distances, and many other
improvements
- r.univar: Parallelization computation extended statistics
- JSON output format support (format="json") in multiple tools (e.g.,
r.report, r.info, v.db.select, t.rast.list, etc.)
- New *grass.jupyter.SeriesMap* class for animating series of vectors or
rasters
- ipyleaflet integration for *grass.jupyter* to create a map in
ipyleaflet and add GRASS data in a single line
- Greatly simplified the creation of new projects in Python (no more
chicken and egg problems) - also in Jupyter notebooks
- GUI: New easy command history navigation through the History browser
panel browser panel 
- GUI: Further improvements of new single-window GUI with undockable map
display window, for a smoother user experience
- New GRASS GIS Programming Style Guide
<https://github.com/OSGeo/grass/blob/main/doc/development/style_guide.md>


**New Addon Tools**  
- i.eodag <https://grass.osgeo.org/grass-stable/manuals/addons/i.eodag.html>: Downloads imagery datasets from various providers through the EODAG API.
- r.flowaccumulation <https://grass.osgeo.org/grass-stable/manuals/addons/r.flowaccumulation.html>: Calculates flow accumulation from a flow direction raster map using the Memory-Efficient Flow Accumulation (MEFA) parallel algorithm by Cho (2023).
- r.fusion <https://grass.osgeo.org/grass-stable/manuals/addons/r.fusion.html>: image fusion, generalized pan-sharpening.
- r.windfetch: addon for computing wind fetch.
- r.maxent.train <https://grass.osgeo.org/grass-stable/manuals/addons/r.maxent.train.html>
- r.maxent.predict <https://grass.osgeo.org/grass-stable/manuals/addons/r.maxent.predict.html>: train, and predict a Maxent model to create a suitability distribution layer.
