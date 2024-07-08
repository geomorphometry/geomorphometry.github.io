---
layout: post
title: "GDEM - a quick assessment"
date: "2021-08-07"
feature-img: "/uploads/img/unsplash/travel.jpeg"
tags: [story,aster,gdem]
published: true
image: false
---

The first 30 m resolution global ASTER-based DEM (GDEM) has recently been released. This is now the most detailed global GIS layer with public access (read more). The GDEM was created by stereo-correlating the 1.3 million-scene ASTER archive of optical images, covering almost 98% of Earth's land surface (claimed 95% vertical accuracy: 20 meters, 95% horizontal accuracy: 30 meters). The one-by-one-degree tiles can be downloaded from NASA's EOS data archive and/or Japan's Ground Data System. The download of DEMs for large areas is at the moment difficult and limited to 100 tiles.

I have downloaded some GDEM tiles for the areas in the Netherlands, Italy, Serbia and USA, and compared these with the most accurate LIDAR-derived DEMs (aggregated to 25 m resolution) available for the same area. The data used for comparison and shown in plot below can be obtained from [**here**]({{site.baseurl}}/uploads/datasets/GDEM_assessment.zip). I was interested to see how accurate is the GDEM and what are the main limitations of using it for various mapping applications.

Conceptually speaking, accuracy of topography (or better to say relief) can be represented by examining (at least) the following three aspects of a DEM:

- _Accuracy of absolute elevations_ (simply the difference between the GDEM and true elevation);
- _Accuracy of hydrological features_ (deviance of stream networks, watershed polygons etc. from true lines);
- _Accuracy of surface roughness_ (deviance of the nugget variation and/or difference in local relief quantified using e.g. difference from the mean value);

![]({{site.baseurl}}/img/posts/Fig_GDEM_comparison.jpg)

Fig: Comparison of the GDEM and LiDAR-based DEMs for four study areas: (1) [fishcamp]({{site.baseurl}}/code_data/datasets/fishcamp); (2) [zlatibor]({{site.baseurl}}/code_data/datasets/zlatibor); (3) calabria, and (4) [boschord]({{site.baseurl}}/2021/07/20/boschoord-case-study) (all maps prepared in resolution 25-30 m).

The results of this small comparison show that:

1. The average RMSE for elevations for these for data sets is: 18.7 m;
2. The average error of locating streams is between 60-100 m;
3. Surface roughness is typically under-represented so that the effective resolution of GDEM is possibly 2-3 times coarser than the actual;

In addition, by visually comparing DEMs for the four case studies, you will notice that GDEM often carries some artificial lines and ghost-like features (GDEM tiles borders, vegetation cover etc.). The worst match between the GDEM and LiDAR-based DEM (reality) is in areas of low relief (boschord). Practically, GDEM looks to be of absolutely no use in areas where the average difference in elevations is <20 m. As the producers of GDEM themselves indicated: "_The ASTER GDEM contains anomalies and artifacts that will reduce its usability for certain applications, because they can introduce large elevation errors on local scales_".

In summary, I can only conclude that (a) there is still a lot of filtering to be done with GDEM to remove the artificial breaks and ghost lines; (b) the effective resolution of the GDEM is probably 60-90 m and not 30 m, hence the whole layer should be aggregated to a more realistic resolution; (c) the first impression is that GDEM is not more accurate than the 90 m SRTM DEM, especially if one looks at the surface roughness and land surface objects. On the other hand, the horizontal accuracy of GDEM is more than satisfactory and GDEM has a near to complete global coverage, so that it can be used to fill the gaps and improve the global SRTM DEM. In addition, the GDEM comes also with a quality assessment (QA) map. Each QA file pixel contains either: (1) the number of scene-based DEMs contributing to the final GDEM value for each 30 m pixel (stack number); or (2) the source data set used to replace identified bad values in the ASTER GDEM.
