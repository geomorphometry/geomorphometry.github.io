---
layout: post
title: "DEMIX reveals which DEMs perform best"
date: "2026-08-26"
tags: [story,geomorphometry,DEMIX,contest]
published: true
image: false
---

First round of the DEMIX exercise published final report

Global digital elevation models (DEMs) have become routine operational inputs across mapping, environmental monitoring, modelling and Earth-observation workflows. Their broad coverage and global availability have made them data that many practitioners simply take for granted. But knowledge of the terrain and topography of Earth’s surface is fundamental for monitoring and understanding terrestrial ecosystems and the planet’s habitability. For that reason, the CEOS Working Group on Calibration and Validation (WGCV) maintains a subgroup dedicated to digital topography and the quality of DEMs, the ‘Terrain Mapping Sub-Group (TMSG). 

DEMs are representations of elevation in the form of a georectified grid, at global scale commonly derived from space-based interferometric synthetic aperture radar (InSAR) or stereoscopic optical observations, while regionally and locally airborne Laser induced detection and ranging (LIDAR) has become the primary source. DEMs can be classified as digital surface models (DSMs) when depicting the lower surface of the atmosphere or digital terrain models (DTMs) when depicting the top of the lithosphere (the Earth’s crust).

A wide variety of DEM products exist – each having different characteristics which suit different applications. It can be challenging to understand which of the available DEM products are fit for purpose for certain applications or regions. That is the practical gap addressed by the Digital Elevation Model Intercomparison Exercise (DEMIX) undertaken by TMSG. By exposing where widely used global DEMs agree, where they differ and how those differences affect rankings, the exercise delivered evidence to users for selecting a DEM rather than defaulting to one by habit.

DEM products were compared through a ‘wine contest,’ which identified requirements of openness, reproducibility, adaptability, and statistical rigour. The characteristics, evaluations, and ranking for each DEM were collected in a GIS database with over 50,000 entries. A quantitative assessment was carried out for each global DEM based on pixel-by-pixel differences of geomorphometric parameters against finer spatial resolution (1-5 m resolution) reference DEMs.

The study incorporates an unprecedented amount of high quality reference data covering a broad range of landforms and surface types, comparing their characteristics without resampling or interpolation. Users are invited to consult the results of DEMIX in order to make informed choices when needing to use a DEM, or in some cases a combination of the most relevant DEMs for their applications.

The final rankings of the wine contest, presented below, compared the six DEMs based on land cover (forest, urban, or barren), slope (cliff, steep, gentle, or flat), differences in elevation, slope and roughness, and statistical metrics.

Led by the European Commission’s Joint Research Centre (JRC), the CEOS Working Group on Calibration and Validation (WGCV) Terrain Mapping Subgroup (TMSG) established DEMIX in partnership with the International Society for Geomorphometry. Several members of the International Society of the Geomorphometry contributed significantly and we hosted various secssions at our latest conference. The exercise was performed over a three-year period starting in 2020, with community-wide calls for participation and an assembly of experts producing a number of peer-reviewed publications, culminating with a JRC reference report published in July 2026.

The objective of DEMIX was to propose a procedure to rank the available free and open global DEMs, taking into consideration user needs while promoting the implementation of FAIR (Findable, Accessible, Interoperable and Reusable) principles. The exercise compared DEMs based on criteria for land cover and terrain slope categories, representative testing, and a statistically sound ranking approach. The report outputs tailored recommendations regarding available DEM products that are not limited to one domain, geographic area, or landscape type, with flexibility for different user needs and applications.

A major challenge in the comparison of the global DEMs were the varying formats, data, and metadata contents. The adoption of a common set of standards would enhance the quality and interoperability of global DEMs and streamline the exchange and utilisation of DEM data for both providers and users. DEMIX makes the following recommendations for data providers:

● Adopt a standardised grid layout, with complete grid definitions and encodings following ISO/OGC rules.

● Include vertical datum information as part of raster DEM files.

● Clearly indicate the product version in the file names.

● Participate in future DEMIX rounds, which serve as a neutral platform for independently evaluating products before their release.

● Provide high quality, finer resolution, accurate, and multi-temporal elevation data to be used as a reference alongside DEM products.

Global DEMs are indispensable operational geospatial datasets, but they should not be treated as error-free or interchangeable. DEMIX delivered to the global community a systematic and transparent method to help choose elevation products more intelligently and help define what better elevation measurements should look like in the future.

## Further Reading:

Read more in the [DEMIX Final Report](https://dx.doi.org/10.2760/3121340), or see other DEMIX publications below - mainly by our ISG members:

- Benchmarking Elevation Plus Land Surface Parameters Finds FathomDEM and Copernicus DEM Win as Best Global DEMs ([2025](https://doi.org/10.3390/rs17233919])) and subsequent discussion ([2026a](https://doi.org/10.3390/rs18142382), [2026b](http://dx.doi.org/10.3390/rs18142399))  
- Ranking of 10 Global One-Arc-Second DEMs Reveals Limitations in Terrain Morphology Representation [2025](https://doi.org/10.3390/rs16173273)  
- Novel Approach for Ranking DEMs: Copernicus DEM Improves One Arc Second Open Global Topography ([2024](https://doi.org/10.1109/TGRS.2024.3368015))  
- Digital Elevation Models: Terminology and Definitions ([2021](http://dx.doi.org/10.3390/rs13183581))  
- The Digital Elevation Model Intercomparison eXperiment DEMIX, a community-based approach at global DEM benchmarking ([2021](https://doi.org/10.5194/isprs-archives-XLIII-B4-2021-395-2021))  
