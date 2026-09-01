---
layout: post
title: "Whitebox Workflows Next Gen released"
date: "2026-08-31"
tags: [story,software,foss,whitebox,rust]
published: true
image: false
author: C.H. Grohmann
---


Whitebox Workflows Next Gen, a complete rewrite of the Whitebox geospatial analysis platform, is now publicly available for **Python, R, and QGIS**.  

Built from the ground up in pure Rust, Whitebox Next Gen provides more than 700 geospatial analysis tools for geomorphometry, terrain analysis, spatial hydrology, LiDAR processing, remote sensing, vector GIS, and spatial statistics. All three interfaces run on the same high-performance backend, allowing users to work in scripts, notebooks, statistical workflows, or a familiar desktop GIS environment.   

Whitebox Next Gen is not an incremental update to the previous Whitebox architecture. It replaces the earlier monolithic system with a modular, full-stack geospatial platform. Core capabilities for raster and vector I/O, coordinate systems and reprojection, vector topology, spatial indexing, LiDAR processing, and other foundational operations are implemented directly within the Whitebox codebase rather than delegated to external C or C++ GIS libraries. This approach provides consistent cross-platform behaviour, fewer system-level dependencies, tighter control over performance and correctness, and greater flexibility for continued research and development  

**Highlights**
- More than 700 tools for geomorphometry, hydrology, LiDAR, remote sensing, vector analysis, spatial statistics, and general geospatial processing
- Publicly available interfaces for Python, R, and QGIS
- A modular, high-performance backend written entirely in Rust, including [wbprojection](https://crates.io/crates/wbprojection), [wbraster](https://crates.io/crates/wbraster), [wbvector](https://crates.io/crates/wbvector), [wblidar](https://crates.io/crates/wblidar), [wbspatialstats](https://crates.io/crates/wbspatialstats), and [wbtopology](https://crates.io/crates/wbtopology) open-source (MIT/Apache licensed) backend libraries
- Most of the 80+ tools that existed within the previous extension product have been migrated to the new Whitebox open core, including the tools for advanced surface curvature analysis and DEM processing
- Native coordinate-reference-system handling and reprojection workflows via [wbprojection](https://crates.io/crates/wbprojection)
- Expanded raster support (19 formats), including GeoTIFF, Cloud-Optimized GeoTIFF (COGs), GeoPackage Raster, and JPEG2000
- Expanded vector support (12 formats), including Shapefile, GeoPackage, FlatGeobuf, GeoParquet, GeoJSON, TopoJSON, and GML
- Modern point-cloud support, including LAS, LAZ, COPC, E57, and PLY
- A dedicated topology engine supporting robust vector analysis, network analysis, route-event workflows, and linear referencing
- Local-first processing on Windows, macOS, and Linux
- A consistent analysis platform across Python scripts and R workflows 
- A newly updated and more advanced QGIS Processing toolbox

Whitebox has particular strengths in terrain analysis, geomorphometry, spatial hydrology, and LiDAR processing. Whitebox Next Gen carries these areas forward while substantially expanding the project’s capabilities for vector analysis, remote sensing, modern spatial data formats, and reproducible geospatial workflows.  

**Get started**
- [Whitebox Next Gen source code on GitHub](https://github.com/jblindsay/whitebox_next_gen)
- [Whitebox Workflows for Python documentation](https://www.whiteboxgeo.com/manuals/api/python/index.html)
- [Whitebox Workflows for R documentation](https://www.whiteboxgeo.com/manuals/api/r/index.html)
- [Whitebox Workflows for QGIS documentation](https://www.whiteboxgeo.com/manuals/qgis/index.html)
- [Install Whitebox Workflows for QGIS](https://plugins.qgis.org/plugins/whitebox_workflows_for_qgis/)
- [Whitebox project website](https://www.whiteboxgeo.com/)

The geomorphometry community is invited to explore Whitebox Next Gen, test its tools and workflows, report issues, and contribute to the continued development of the project.