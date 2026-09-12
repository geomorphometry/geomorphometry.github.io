---
layout: page
title: "Geomorphometry: Concepts, Software, Applications"
permalink: /book/
hero_image: "../uploads/img/headers/header_lanz_2400.jpg"
hero_darken: true
show_sidebar: false
---

<img src="{{site.baseurl}}/uploads/img/books/geomorphometry_2026_book_cover.jpg" width="35%" />  

After a couple of years of work, the second edition of the ISG-driven textbook on geomorphometry is now published! It was well worth the wait; in this book, readers will find the foundational and state-of-the-art techniques behind geomorphometry, the latest software tools for geomorphometric analyses, and several revised and new chapters showcasing applications of geomorphometry. Overall, it introduces nine software options and ten applications, updating and complementing the first edition of the book.  

A total of 55 contributors from our community and beyond and with a wide range of expertise contributed to the book. The book synthesizes modern quantitative land-surface analysis, from data collection to applications, integrating theory, software, and real-world applications. It provides a practical guide to preparing digital elevation models to analyze and extract land-surface parameters and objects. It presents methods for selecting datasets and tools, building reproducible workflows, benchmarking terrain methods, and applying results to mapping, modelling, and decision support.  

Like the first version, the volume is organized in three sections: theoretical concepts, technical implementation (software), and discipline-specific applications. Each of the book’s three sections comprises between nine and twelve chapters. Many chapters overlap in both content and examples, illustrating not only the many types of land-surface parameters or objects that can be derived, but also contrasting how different software can support various applications. Links to external sources and key literature can be found at the end of each chapter, and more than 150 text boxes highlight important remarks throughout the book. The book also includes a comprehensive list of references and an index at the end. A dataset of open geospatial data for the Ponui Island (New Zeland) was assembled and used in many of the examples presented in the book; the dataset is available in Zenodo. As supplementary material, a [GitHub repository][github_repo] is provided with most of the code used for this book.  

To purchase the book or individual chapters, visit the [Elsevier Shop][elsevier_shop].  

If you’re on an academic network, you might have access to the individual book chapters via [ScienceDirect][sciencedirect].  

A Bibtex file containing all the references cited in the book (almost 3,000!), as well as the entries for this edition chapters can be [downloaded here][bibtex_file].  

<br>
Below you can find a short summary of each chapter.   

#### Part I: Concepts

[Chapter 1][chapter_1] aimed to introduce readers to the field of geomorphometry, its basic concepts and principles, and major applications. This introduction is followed by a historical review of the discipline, from the earliest contour lines to the computer programs used to process early DEMs.  

[Chapter 2][chapter_2] is a conceptual and mathematical introduction to modelling the land surface. First, the main types of models of the land surface are presented, as well as their relations with geological, anthropogenic and extraterrestrial processes over time. Next, the chapter addresses local and global mathematical models of the land surface, including vector representations (TINs), regular grid (raster) models, hydrologically corrected DEMs, and the implications of point and areal representations of raster cells. Finally, land-surface analysis algorithms are illustrated by deriving first-, second-, and third-order derivatives to calculate slope, aspect, curvatures, and changes in curvature.  

The most frequently used and contemporary DEM production methods are reviewed in [Chapter 3][chapter_3]. This chapter compares ground- and remote sensing-based techniques and outlines the strengths and weaknesses of DEM data from different sources and methods, including ground-survey techniques, digitization of topographic maps, photogrammetry, lidar, across-track SAR interferometry, acoustic remote sensing, and satellite-derived bathymetry. It also compares key characteristics of different sources.  

[Chapter 4][chapter_4] complements the previous chapter by listing examples of available DEMs, from local and regional to global ones (e.g., SRTM, TanDEM-X, FathomDEM). A section also describes important bathymetric DEMs, and another one presents DEMs from other planetary bodies such as the Moon and Mars. In most cases, it provides links to access the discussed datasets. Finally, the chapter discusses DEM comparisons and offers recommendations based on the DEMIX methodology.  

[Chapter 5][chapter_5] is devoted to techniques for improving the quality of DEMs prior to geomorphometric analysis. After a discussion of the various types of errors in DEMs and their derivatives, several methods to reduce errors are presented, including: horizontal and vertical shift corrections; treatment of local outliers and noise; filtering of water surfaces, surface roughness, and lidar DEMs; filling sinks and voids; geostatistical and Monte-Carlo simulations; mosaicking of adjacent DEMs; and use of auxiliary data and machine learning.  

[Chapter 6][chapter_6] provides an overview of "basic" land-surface parameters (LSPs), measures derived directly from DEMs without additional input. The chapter divides the LSPs by their local (focal) and regional (zonal) GIS operations. Local operations are described by the order of the partial derivatives of the topographic surface: first order (elevation gradient, slope, aspect, hillshade, openness), second order (curvatures), and third order (change in curvature). Surface roughness is considered in the broader sense as surface complexity or texture, and the chapter lists several approaches for calculating this measure. Regional LSPs include the organization (or anisotropy) of terrain and viewsheds. The chapter also discusses LSP visualization, multi-scale calculation, reproducibility, and naming.  

[Chapter 7][chapter_7] describes hydrological land-surface parameters for quantifying water flow and related surface processes. This overview guides readers through key concepts such as flow lines, flow direction, and contributing area, as well as preparing DEMs for hydrological analysis. The chapter details flow-route (dispersive and nondispersive) and flow-accumulation algorithms, and illustrates LSPs based on catchment areas and flow lines, as well as land-surface objects based on flow variables (river networks, drainage divides, and watersheds).  

[Chapter 8][chapter_8] provides an extensive review of solar radiation models and approaches to quantifying the land surface’s exposure to climatic influences. First, it details the relationship between topography and radiation. Next, topo-climatic modelling is extended to the estimation of land surface temperature, precipitation, snow cover, and exposure to wind and cold-air flow. Lastly, the chapter presents the representation of topography in climate models and spatial model discretization.  

Finally, [Chapter 9][chapter_9] introduces landform as a conceptual entity and defines it based on topographic geometry, followed by a discussion of its recognition at different scales. It then describes techniques for classifying landform elements based on curvature, their relative position in the landscape, and computer vision algorithms. The concept of geometric signature is introduced, along with schemes for classifying landform types.  

<img src="{{site.baseurl}}/uploads/img/books/fig_ch9.jpg" width="60%" />   
Examples 16-fold landform types for Ponoui Island, according to Iwahashi and Pike (2007). This is figure 9.8 in [Chapter 9][chapter_9].

<br>

#### Part II: Software 

[Chapter 10][chapter_10] opens the middle third of the book with a general inventory and prospect of several packaged computer programs suited to geomorphometry, including software not demonstrated in this book. It also includes a short discussion of how the software landscape has evolved since the 2000s.   

The remaining chapters in Part II illustrate eight well-known packages currently available for land-surface analysis, ranging from proprietary (ArcGIS, [Chapter 11][chapter_11]; RiverTools, [Chapter 18][chapter_18]) to mixed (TopoToolbox, [Chapter 16][chapter_16]; Whitebox, [Chapter 17][chapter_17]) and open-source (GRASS, [Chapter 12][chapter_12]; MICRODEM, [Chapter 13][chapter_13]; QGIS/PCRaster, [Chapter 14][chapter_14]; SAGA, [Chapter 15][chapter_15]) software. Six of these chapters are authored by the software’s original developers, and two by later developers or expert users. Most chapters present some of these elements: a short description of the software, its origins and target users; how to acquire and install the package; what it can or cannot do; how to get technical support; how to import and display DEMs; which land-surface parameters and objects can be derived from the package, and how they are calculated; how particular land-surface parameters and objects can be interpreted and applied; and in some cases, a summary of the strengths and weaknesses of the software and the authors’ expectations for what the software might become in the future. The final chapter in this part of the book, [Chapter 19][chapter_19], does not focus on a specific software package but instead on open-source programming languages that enable conducting geomorphometric analyses, which have gained significant traction since the first version of this book.  

<img src="{{site.baseurl}}/uploads/img/books/fig_ch18.jpg" width="60%" />   
Some hillshaded and contrast-enhanced plots showing gridded properties of the south river
of Ponui Island. This is figure 18.10 in [Chapter 18][chapter_18].

<br>

#### Part III: applications 

The final section of the book exemplifies the role of geomorphometry in other sciences. The section starts with [Chapter 20][chapter_20], which provides an overview of the role of digital land surface analysis in creating maps and models across a broad spectrum of disciplines. The chapter explains why DEM analysis has become so essential for quantifying and understanding the natural landscape and provides an overview of the characteristics of the various case studies presented in the other chapters of this section.   

The subsequent chapters of Part III describe specific applications of DEM analysis to generate and interpret spatial information in various disciplines, including soil mapping ([Chapter 21][chapter_21]), geomorphology ([Chapter 22][chapter_22]), mass movement modelling ([Chapter 23][chapter_23]), ecology ([Chapter 25][chapter_25]), hydrological modelling ([Chapter 26][chapter_26]), and archaeology ([Chapter 27][chapter_27]). [Chapter 24][chapter_24] explains how machine learning and computer vision can contribute to these applications, and [Chapter 28][chapter_28] discusses how climate change might affect the modelled landscape and how geomorphometry can help study those effects. [Chapter 29][chapter_29] presents an overview of applications that use underwater DEMs, and [Chapter 30][chapter_30] introduces readers to planetary DEMs and extraterrestrial geomorphometry. Most chapters address the following topics: an introduction to the state of the art of the application; an explanation of the importance of geomorphometry in the field; an example case study; and a summary of the opportunities and challenges of applying geomorphometry in the described context.   

Finally, the book concludes with [Chapter 31][chapter_31], which examines how geomorphometry applications have evolved since the first version of the book and what we expect to happen in the next decade or so. Finally, book contributors provided their perspective on questions such as "What breakthroughs might emerge from future advances in technology?", and "Which concepts, applications, and societal needs are likely to drive the discipline in the next few years?."


<img src="{{site.baseurl}}/uploads/img/books/fig_ch31.jpg" width="45%" />   
The space-time continuum of Geomorphometry - space, time, hyper/multi-spectral, resolution,
multi-scale facets of results which need to be taken into account. This is figure 31.1 in [Chapter 31][chapter_31].



<br>

##### Book info:
Geomorphometry: Concepts, Software, Applications   
(Developments in Soil Science, Volume 37)  
Edited by: Hannes I. Reuter, Carlos Henrique Grohmann, Vincent Lecours  
Publisher: Elsevier  
Publication date: 2026  
Edition: 2nd  
Language: English  
Print length: 1064 pages  
ISBN-10: 0443333769  
ISBN-13: 978-0443333767  
DOI: [https://doi.org/10.1016/c2023-0-52503-0](https://doi.org/10.1016/c2023-0-52503-0)  






[github_repo]: <https://github.com/geomorphometry/geomorphometrybook>
[zenodo_ponui]: <https://doi.org/10.5281/zenodo.18314107>
[bibtex_file]: <{{site.baseurl}}/uploads/docs/geomorphometry_book_2026.bib>
[elsevier_shop]: <https://shop.elsevier.com/books/geomorphometry/reuter/978-0-443-33376-7>
[sciencedirect]: <https://www.sciencedirect.com/bookseries/developments-in-soil-science/vol/37/suppl/C>
[chapter_1]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00011-2>
[chapter_2]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00012-4>
[chapter_3]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00013-6>
[chapter_4]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00014-8>
[chapter_5]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00015-X>
[chapter_6]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00016-1>
[chapter_7]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00017-3>
[chapter_8]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00018-5>
[chapter_9]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00019-7>
[chapter_10]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00021-5>
[chapter_11]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00022-7>
[chapter_12]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00023-9>
[chapter_13]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00024-0>
[chapter_14]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00025-2>
[chapter_15]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00026-4>
[chapter_16]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00027-6>
[chapter_17]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00028-8>
[chapter_18]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00029-x>
[chapter_19]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00030-6>
[chapter_20]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00032-X>
[chapter_21]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00033-1>
[chapter_22]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00034-3>
[chapter_23]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00035-5>
[chapter_24]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00036-7>
[chapter_25]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00037-9>
[chapter_26]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00038-0>
[chapter_27]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00039-2>
[chapter_28]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00040-9>
[chapter_29]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00041-0>
[chapter_30]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00042-2>
[chapter_31]: <http://dx.doi.org/10.1016/B978-0-44-333376-7.00043-4>