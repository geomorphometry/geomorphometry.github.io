---
layout: post
title: "Coffee Talk - FathomDEM, a new global 30 m DTM"
date: "2025-03-11"
tags: [story,event,gct,Coffee-Talk]
published: true
image: false
---

**FathomDEM, a new global 30 m DTM**



Dr. Chris Lucas  
Fathom company  
<img src="{{site.baseurl}}/uploads/img/faces/chrislucas.png" width="25%" />

January 20th, 2026  
14:00 (UTC)

 Recording available in our [YouTube channel][video_chrislucas] <!-- add after video uploaded -->

**Bio:** Chris Lucas is the Principal Machine Learning Engineer at Fathom, a global water intelligence company. Holding a PhD in High Energy Physics, his 11 years in industry span from software engineering to ML research, contributing to projects such as scaling medical diagnosis models and developing new computer vision techniques for vehicle analysis. At Fathom, he leverages his combined ML, software, and scientific expertise to advance multiple levels of the company's modeling stack, from terrain modeling (DEMs) to generative AI for climate downscaling and hydrological modeling with graph neural networks.  

**Abstract:** Accurate digital elevation models (DEMs) are foundational inputs for a vast array of geomorphometry applications, including natural hazard modeling, glaciology, and infrastructure planning. However, existing global DEMs, such as Copernicus DEM (COPDEM), often contain surface features like trees and buildings, limiting their effectiveness as Digital Terrain Models (DTMs). This talk introduces FathomDEM, a new global 30 m DTM created using a novel machine-learning methodology. We utilized a hybrid vision transformer model within a U- Net architecture to perform pixel-wise regression, analyzing and correcting the height biases in COPDEM. This approach differs significantly from previous methods (like the pixel-by-pixel correction used for FABDEM) by leveraging 2D spatial information (context) as an inductive basis, essentially employing 'computer vision' to achieve more spatially coherent and robust corrections. FathomDEM was trained on extensive, diverse LiDAR reference data and has been rigorously validated, demonstrating: Improved Accuracy, surpassing the accuracy of existing best-ranked global DEMs; Excellent Performance in Specific Landscapes, showing reduced error even when compared to specialized coastal DEMs (e.g., DeltaDTM); High Utility in Downstream Tasks, when utilised in flood inundation modeling, FathomDEM achieves increased accuracy, approaching the performance levels of models derived from high-resolution LiDAR data. Join this session for an informal discussion on the methodology behind FathomDEM, its novel use of ML for artifact removal, and its potential to improve applied
geomorphometry tasks globally.    


[video_chrislucas]: <https://www.youtube.com/watch?v=styhRiQdRPo> 
<!-- update after video uploaded -->


