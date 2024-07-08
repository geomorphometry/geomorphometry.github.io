---
layout: post
title: "New Parallel version of Hydrologic Terrain Analysis Software TauDEM"
date: "2012-03-05"
feature-img: "/uploads/img/unsplash/travel.jpeg"
tags: [story,hydro,software,arcgis]
published: true
image: false
---

![]({{site.baseurl}}/uploads/img/posts/taudem_preview.jpg)

Geomorphometry followers may be interested in the new version of my TauDEM (Terrain Analysis Using DEMs) software available from [http://hydrology.usu.edu/taudem](http://hydrology.usu.edu/taudem).

TauDEM is free and open source. It comprises a set of Digital Elevation Model (DEM) tools for the extraction and analysis of hydrologic information from topography as represented by a DEM.

The new version, TauDEM 5.0 takes advantage of parallel programming using the message passing interface (MPI) and achieves improved runtime efficiency and the capability to run larger problems.

TauDEM includes functions for the development of hydrologically correct (pit removed) DEMs, calculation of flow paths, contributing area, stream networks and other flow related derived information.  Its unique features are that it uses the D-Infinity flow model for evaluation of information derived from dispersed flow over hillslopes and provides objective methods for the determination of stream network delineation thresholds.

The parallel version (TauDEM 5.0) has been completely restructured as a set of command line functions in standard C++ using MPICH2.  The source code has been compiled for both PC's and parallel clusters.  GeoTiff is used as the input/output file format so that the command line functions that provide core functionality are platform independent.  TauDEM does include an ArcGIS toolbox Graphical User Interface (for ArcGIS 9.3.1) that has been recoded to use system calls to these command line executables.  

The development of TauDEM 5.0 was supported by the US Army Engineer Research and Development Center under contracts W9124Z-08-P-0420 and W912HZ-09-C-0112.
