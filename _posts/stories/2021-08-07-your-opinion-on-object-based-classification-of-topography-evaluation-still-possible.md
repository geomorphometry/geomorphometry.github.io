---
layout: post
title: "Your opinion on object-based classification of topography - Evaluation still possible!"
date: "2021-08-07"
tags: [story,obia,poll]
published: true
image: false
---

**WEB APPLICATION** and **QUESTIONNAIRE** at **http://zgis205.plus.sbg.ac.at/PhysiographicClassificationApplication/default.aspx**

**Dear colleagues,** We kindly ask for your help in evaluating the preliminary outputs of a global physiographic classification. The methodology has been designed for general purposes. We hope, however, that the results can be tuned to specific applications, by using the object attributes, without a need of running the classification again. Potential domains of application include Landscape Ecology, Ecology, Geomorphology, Geology, Hydrology, Soil Science, and Agriculture. Your evaluation would be useful in improving the current classification. The results of your evaluation will be part of a paper we intend to submit to a peer-reviewed journal. Classification results are embedded within a **web application** available at the following address

##### **http://zgis205.plus.sbg.ac.at/PhysiographicClassificationApplication/default.aspx**.

You can visualize the results and let us know your opinion by **filling in the form under the red button** named ‘Please provide your feedback here.’ Apart of the classification itself, i.e. to which degree classes describe correctly given regions, we would like you evaluating the quality of object boundaries, i.e. to which degree boundaries match topographic discontinuities. After evaluation, both the database and the tool will be released for free download.

**Please find below additional details on the methods and the web application.**
 <!--more-->
**Methodology**

We introduce an object-based method to automatically classify topography from SRTM data. The new method relies on the concept of decomposing land-surface complexity into more homogeneous domains. An elevation layer is automatically segmented and classified at three scale levels that represent domains of complexity by using self-adaptive, data-driven techniques. For each domain, scales in the data are detected with the help of local variance and segmentation is performed at these appropriate scales. Objects resulting from segmentation are partitioned into sub-domains based on thresholds given by the mean values of elevation and standard deviation of elevation respectively. The method is simple and fully automated. The input data consists of only one layer, which does not need any pre-processing. Both segmentation and classification rely on only two parameters: elevation and standard deviation of elevation. Unlike cell-based methods, results are customizable for specific applications; objects can be re-classified according to the research interest by manipulating their attributes. The tool can be applied to any regional area of interest and can also be easily adapted to particular tasks. Both segmentation and class thresholds are relative to the extent and characteristics of the dataset. Therefore, when applying the tool to regional/national levels, the results should be interpreted within the appropriate context (e.g. ‘High Mountains’ that may result from classification of Dutch territory are just the highest and roughest areas relative to this extent). To show the differences, we added the results of classification at the level of the Austrian territory to the web application.

**Web application**

##### **http://zgis205.plus.sbg.ac.at/PhysiographicClassificationApplication/default.aspx**

You will find the following **layers**:

1. _Global\_Level3_. This is the finest scale at the global level. Object boundaries are transparent to enhance visualization at full extent;

2. _GlobalLevel\_objectsEvaluation_. This is the same layer as above, with object boundaries on. It helps in evaluating the match with land-surface discontinuities;

3-5. _Results of classification of the Austrian territory at all scale levels_;

6. _Country Boundaries_ - for orientation;

7. _ESRI\_ShadedRelief_ \- to visualize topography. Please be aware that this classification was obtained form SRTM data at approximately 1 km resolution, while the shaded relief map is much finer in some areas (see http://server.arcgisonline.com/ArcGIS/rest/services/ESRI\_ShadedRelief\_World\_2D/MapServer). Therefore, some discrepancies might be apparent.

For each layer, except for the 7th, objects can be selected using the info button. After activating it, click within a polygon: a pop-up window will display the class label of the polygon, as well as its attribute table. Click on ‘_Add to results_’ at the bottom of the pop-up window: the polygon is selected. The attributes are presented in the table below; for details and equations see the eCognition Reference Book.

The following eleven attributes are listed for each object:

- **Area\_Pxl**: Area in pixels. 1 pixel is approximately 1sq km
- **Asymmetry**: Relative length compared to a regular polygon
- **Compactness**: Product of length and width, divided by the number of pixels
- **Elliptic\_F**: Elliptic fit. Describes how well an image object fits into an ellipse of similar size and proportions.
- **LengthWidt**: Length/Width ratio of an image object
- **Local\_Reli**: Ratio. Max elevation minus Min elevation within a polygon
- **Mean\_Layer**: Mean elevation of cells within a polygon
- **Roundness**: Describes how similar an image object is to an ellipse. It is calculated by the difference of the enclosing ellipse and the enclosed ellipse.
- **Shape\_inde**: Shape index. Describes the smoothness of a polygon border
- **Skewness\_L**: Skewness of elevation (based on cells within a polygon)
- **Standard\_d**: Standard deviation of elevation (based on cells within a polygon)

**Thank you for your help!**
