---
layout: post
title: "Continental Europe Digital Terrain Model at 30 m resolution based on multisource data"
date: "2021-08-12"
tags: [story,publication,dataset]
published: true
image: false
---

Within the **[OpenDataScience.eu](https://maps.opendatascience.eu/?base=OpenStreetMap%20(grayscale)&layer=Topographic%20index%20(wetness%20index)&zoom=4.8&center=45.3356,9.9145&opacity=45)** (Geo-harmonizer) project we have recently produced an Digital Terrain Model for Continental Europe based on the four publicly available Digital Surface Models:  [MERITDEM](http://hydro.iis.u-tokyo.ac.jp/~yamadai/MERIT_DEM/), [AW3D30](https://www.eorc.jaxa.jp/ALOS/en/aw3d30/index.htm), [GLO-30](https://spacedata.copernicus.eu/web/cscda/dataset-details?articleId=394198), [EU DEM](https://www.eea.europa.eu/data-and-maps/data/copernicus-land-monitoring-service-eu-dem). This is basically an Ensemble Machine Learning approach where GEDI level 2B points (Level 2A; "elev\_lowestmode") and ICESat-2 (ATL08; "h\_te\_mean") were used to train a multisource model to predict "most probable height of terrain" including the prediction errors per pixel.

So which of the four big global DEM's is the best match with terrain heights? Our results indicate that it is the [MERITv1.0.1](http://hydro.iis.u-tokyo.ac.jp/~yamadai/MERIT_DEM/) (originally available at 90-m, but was downscaled here to 30-m using cubic splines) followed by the AW3Dv2012 and GLO-30. This confirms that Yamazaki et al. (2017) have done an excellent work in filtering out canopy and artifacts in the original SRTM/AWD30 data.

Read more about MERIT DEM in:

- Yamazaki D., D. Ikeshima, R. Tawatari, T. Yamaguchi, F. O'Loughlin, J.C. Neal, C.C. Sampson, S. Kanae & P.D. Bates, (2017). [A high accuracy map of global terrain elevations](http://onlinelibrary.wiley.com/doi/10.1002/2017GL072874/full). Geophysical Research Letters, vol.44, pp.5844-5853, 2017 doi: [10.1002/2017GL072874](https://doi.org/10.1002/2017GL072874)

To access the Continental Europe Digital Terrain Model at 30-m please visit https://maps.opendatascience.eu and select "terrain" from the layer menu.

You can also download the DTM for EU including the regression matrix with all training points (GEDI/ICESat) via:

- Hengl, T., Leal Parente, L., Krizan, J., & Bonannella, C. (2020). [Continental Europe Digital Terrain Model at 30 m resolution based on GEDI, ICESat-2, AW3D, GLO-30, EUDEM, MERIT DEM and background layers (v0.3)](https://zenodo.org/record/4724549) \[Data set\]. Zenodo. https://doi.org/10.5281/zenodo.4724549

![]({{site.baseurl}}/uploads/img/data/eu_ensemble_dtm_preview_odsEurope.jpg)