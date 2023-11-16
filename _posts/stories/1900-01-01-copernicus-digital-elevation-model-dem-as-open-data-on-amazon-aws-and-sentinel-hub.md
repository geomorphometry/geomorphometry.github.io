---
layout: post
title: "Copernicus Digital Elevation Model (DEM) as Open Data on Amazon AWS and Sentinel-Hub"
date: "2021-08-12"
feature-img: "/uploads/img/unsplash/travel.jpeg"
tags: [story,copernicus,dataset]
published: true
image: false
---

European Space Agency (ESA) has recently made available two global Digital Surface Models:

- GLO-30: the 30-m spatial resolution DSM,
- GLO-90: the 90-m spatial resolution DSM,

Both are available for download from [**cdsdata.copernicus.eu**](https://spacedata.copernicus.eu/data-offer/core-datasets) on a free basis for the general public under the terms and conditions of the Licence found [here](https://spacedata.copernicus.eu/documents/20126/0/CSCDA_ESA_Mission-specific+Annex.pdf).

A copy of the GLO-30 and GLO-90 is now also available as Cloud Optimized GeoTIFFs from the [**Amazon AWS public data repository**](https://registry.opendata.aws/copernicus-dem/). The visualization shown above is from the [sentinel-hub.com](https://apps.sentinel-hub.com/eo-browser/?zoom=12&lat=41.7726&lng=12.29198&themeId=DEFAULT-THEME&visualizationUrl=https%3A%2F%2Fservices.sentinel-hub.com%2Fogc%2Fwms%2F6448ffd0-56c5-4601-bed7-242bf75d97db&datasetId=DEM_COPERNICUS_30&fromTime=2021-08-12T00%3A00%3A00.000Z&toTime=2021-08-12T23%3A59%3A59.999Z&layerId=COLOR).

To learn more about the GLO-30 and it's accuracy and production, refer to [this article](https://spacedata.copernicus.eu/web/cscda/dataset-details?articleId=394198).


![]({{site.baseurl}}/uploads/img/posts/eo_browser_dem_copernicus.jpg)