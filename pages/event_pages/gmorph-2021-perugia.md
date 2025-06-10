---
layout: page
title: Geomorphometry 2021 - Perugia, Italy
permalink: /2021/
hero_image: "../uploads/img/headers/pexels-pixabay-35577022.jpg"
hero_darken: true
show_sidebar: false
---

{% include image-modal_fx.html ratio="is-3by1" link="/uploads/img/groups_modal/geomorphometry_2021_group_photo_zoom_3by1.jpg" alt="Happy faces" %} 



### Original Conference Website: [http://geomorphometry2021.org](http://geomorphometry2021.org)

## Summary 
 
About 50 researchers from around the world attended the event, mostly by remote connection. The conference only featured oral sessions, with 44 contributions. Three invited keynote talks, by Michael Hutchinson (Australian National University College of Science), Igor Florinsky (Russian Academy of Sciences) and Marco Cavalli (CNR IRPI, Padua) enriched the content of the conference. [Contributions](http://geomorphometry2021.org/index.php/scientific-program) were spread over three days, grouped by topic: “use of digital elevation, terrain and surface models” on day 1, “dynamics of earth surface: automated surface analysis and modelization” on day 2, and “modeling geomorphological processes” on day 3.

All of the sessions demonstrated that quantitative analysis of the Earth's surface is closely related to the scale at which the surface itself is described/represented. Research on a global scale (_e.g._ aimed at the definition of accurate hydrographic networks) was counterbalanced by studies that focused on centimetric portions of Earth's surface (_e.g._ small plates where accretion of tufa/travertine is studied). A related relevant topic was the comparison of lidar data with global (or quasi-global) DEMs and among different global DEMs, using different methods in many study areas. Explicit comparisons highlighted that, in selected areas representative of most existing settings, Copernicus DEM is the best performing; other comparisons in different areas and methods favored MERIT DEM. In all cases, lidar data represents the benchmark. Despite that, a discussion highlighted that peculiar applications may not be so sensitive to details represented in elevation data from lidar and/or SfM measurements to justify the much higher cost. There also have been an explicit proposal to merge global and local elevation data, already existing and available online for Europe.

This also lead to a discussion about the characteristic scale of terrain analysis, and a few presentations described multi-scale approaches as mature tools for a variety of application. Mainly, they described multi-scale methods for estimation of terrain roughness, curvatures, and landform mapping. The relationship between multi-scale approaches and characteristic scale may lead to need of optimization of numerical parameters for terrain analysis and classification.

A few presentations focused on the geomorphological and physical meaning of maps derived from digital terrain models (such as curvatures) or on the definition of new functions aimed at representing the topology of surface water flow directions or the selection of features (derived from DEM) which are relevant in supervised classification applications.

Applications of geomorphometry concepts and algorithms to other disciplines/topics have been numerous and included tectonics, soil erosion, landslide susceptibility, thermokarst phenomena, river forms, coastal habitat and coastal dunes, crevasses in polar ice, inundated areas, glacial cirques and volcanic eruptions.

One addition to the topics of this year’s edition of the conference was specifically commercial and industrial application. The scientific program actually included a few contributions explicitly reporting about industrial processes (microscopic analysis of silicon wafer “topography”) and commercial applications (deposition and analysis of submarine cables, rockfall susceptibility along the Italian national railway). Other contributions, even if not specifically commercial, highlighted the use of algorithms borrowed from computer graphics for terrain segmentation, and adaptation of general purpose software for marine geomorphometry. Moreover, commercial and industrial applications were one of the key topics – along with the role of local/global elevation data – for a proposed session at the upcoming European Geoscience Union General Assembly, prepared by a few of the participants of Geomorphometry 2021.

Contributions presented at the conference are available as peer-reviewed short papers from the [book of Proceedings](https://doi.org/10.30437/geomorphometry2020) of the 2020 submissions (CNR Edizioni, Rome), or on [Zenodo](https://zenodo.org/communities/geomorphometry/?page=1&size=20), for new submissions. Most of the presentations are also available as PDF and/or video recording at the [conference website](http://geomorphometry2021.org); a few of the contributions also have a link to published papers, either on the special issue “Advances in geomorphometry” in the journal [Transaction in GIS](https://onlinelibrary.wiley.com/loi/14679671).

![]({{site.baseurl}}/uploads/img/meet2021/summary_pic5.jpg)  
The beautiful city of Perugia


![]({{site.baseurl}}/uploads/img/meet2021/geomorphometry_2021_group_photo.jpg)  
In-person attendance to the conference



### Book of Proceedings
Massimiliano Alvioli, Ivan Marchesini, Laura Melelli, and Peter Guth (2020)  
Proceedings of the Geomorphometry 2020 Conference, Perugia, Italy  
CNR Edizioni, 270 p.  
Book DOI: [10.30437/geomorphometry2020](https://doi.org/10.30437/geomorphometry2020)  
ISBN: 978 88 8080 282 2  
ISBN 978 88 8080 410 9 (updated version)  

### Transactions in GIS special issue:  
[https://onlinelibrary.wiley.com/toc/14679671/2021/25/5](https://onlinelibrary.wiley.com/toc/14679671/2021/25/5)



## Scientific Commitee	

- Alexander Brenning - Friedrich Schiller University
- A-Xing Zhu - University of Wisconsin
- Carlos Grohman - University of Sao Paolo
- Hannes I. Reuter - European Commission
- Helena Mitasova - North Carolina State University
- Ian Evans - Durham University
- Jaroslav Hofierka - Pavol Jozef Safarik University
- John Gallant - CSIRO
- John Lindsay - University of Guelph
- Lucian Dragut - West University of Timisoara
- Massimiliano Alvioli - CNR IRPI Perugia
- Mihai Niculita - University Al. I. Cuza
- Peter L. Guth - US Naval Academy
- Qiming Zhou - Hong Kong Baptist University
- Qin Cheng-Zhi C- hinese Academy of Sciences
- Robert A. MacMillan - LandMapper Environmental Solutions Inc.
- Samantha Arundel - USGS
- Scott D. Peckham - University of Colorado
- Steve Kopp - ESRI
- Tomislav Hengl - OpenGeoHub Foundation
- Vincent Lecours, Université du Québec à Chicoutimi, Canada  


## Organizing Commitee
- Massimiliano Alvioli - CNR IRPI Perugia
- Ivan Marchesini - CNR IRPI Perugia
- Laura Melelli - University of Perugia
- Peter L. Guth - US Naval Academy




## Scientific Program


### SEPTEMBER 13: USE OF DIGITAL ELEVATION, TERRAIN AND SURFACE MODELS

|10.00        | Opening connections|
|10.15        | **Conference opening** |
|10.30-10.45  |Jozef Minár, Marián Jenčo and Ian S. Evans <br> [What does land surface curvature really mean?](https://doi.org/10.30437/geomorphometry2020_6) <br> [video](https://youtu.be/mUwotbzEVgQ) |
|10.45-11.00  | Cheng-Zhi Qin, Peng Liang and A-Xing Zhu <br> [Two case-based classification strategies of automatically selecting terrain covariates for building geographic variable-environment relationship](https://doi.org/10.30437/geomorphometry2020_9) <br> [presentation](https://zenodo.org/record/5503584) <br> [video](https://youtu.be/qU3WKOn_xro) |
|11.00-11.15  | Fran Domazetović, Ante Šiljeg and Ivan Marić <br> [Guidelines for optimization of terrestrial laser scanning surveys over gully erosion affected areas](https://doi.org/10.30437/geomorphometry2020_59) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Domazetovic.pdf) <br> [video](https://youtu.be/-f3ENoPf1-U) |
|11.15-11.30  | Alexey Victorov, Olga Trapeznikova and Timofey Orlov <br> [Probabilistic behavior modeling of morphometric parameters for thermokarst plains with fluvial erosion in Cryolithozone](https://doi.org/10.30437/geomorphometry2020_70) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Victorov.pdf) <br> [video](https://youtu.be/UCIzGa3RrHo)|
|11.30-11.45  | Break time|
|11.45-12.15  | **Keynote talk: Marco Cavalli, Stefano Crema and Lorenzo Marchi** <br> [Sediment connectivity assessment through a geomorphometric approach: review of recent applications](https://doi.org/10.30437/geomorphometry2020_57) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Cavalli.pdf) <br> [video](https://youtu.be/f6kx2jt_f3s)|
|12.15-12.30  | John Gallant <br> [The surface stream function: representing flow topology with numbers](https://doi.org/10.30437/geomorphometry2020_60) <br> [video](https://youtu.be/LK4HF1wrIzY)|
|12.30-12.45  | John Gallant<br>[The D8 implementation of the surface stream](https://doi.org/10.30437/geomorphometry2020_61)<br>[video](https://youtu.be/0oU6CqTjGjk)
|12.45-13.00  | Discussion and Conclusion|
|13.00-14.00  | Lunch time|
|14.00-14.15  | Marina Metes, Kristina Hopkins, Labeeb Ahmed, Sam Lamont, Peter Claggett and Greg Noe <br> [Mapping stream and floodplain geomorphic characteristics with the Floodplain and Channel Evaluation Tool (FACET) in the Mid-Atlantic Region, United States](https://doi.org/10.30437/GEOMORPHOMETRY2020_65) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Metes.pdf) <br> [video](https://youtu.be/Ddnf95cpJRM) |
|14.15-14.30  | Adeyemi Olusola <br> [Lithology and channel network initiation and orientation: a case study of upper Ogun River Basin, Soyhwestern Nigeria](https://doi.org/10.30437/geomorphometry2020_66) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Olusola.pdf) <br> [video](https://youtu.be/Mh53hJAhHsM) |
|14.30-14.45  | Priyank Patel, Sayoni Mondal and Rajarshi Dasgupta <br> [Morphometric and channel erosivity analysis of lateritic gully catchments using high resolution DTM and repeat survey Structure-from-Motion datasets](https://doi.org/10.30437/geomorphometry2020_67) <br>[published as full paper in Transactions in GIS](https://doi.org/10.1111/tgis.12828) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Patel.pdf)|
|14.45-15.00  | Francesco Bucci, Michele Santangelo, Francesco Mirabella, Andrea Mazzoni and Mauro Cardinali <br> [Drainage inversion revealed by geomorphometric analysis of fluvial terraces](https://doi.org/10.30437/geomorphometry2020_56) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Bucci.pdf) <br> [video](https://youtu.be/SCqYY5Tyqac) | 
|15.00-15.15  | Break time|
|15.15-15.30  | Mihai Niculita <br> [Burial mound detection using geomorphometry and statistical methods: pixels versus objects](https://doi.org/10.30437/geomorphometry2020_7) <br>[presentation](https://zenodo.org/record/5502986) <br> [video](https://youtu.be/U-iLHNZS53Y) |
|15.30-15.45  | Richard Feciskanin and Jozef Minár <br>  [An optimization of triangular network and its use in DEM generalization for the land surface segmentation](https://doi.org/10.30437/GEOMORPHOMETRY2020_2) <br>[published as full paper in Transactions in GIS](https://doi.org/10.1111/tgis.12796) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Feciskanin.pdf) <br> [video](https://youtu.be/pwo_3KucPKU) |
|15.45-16.00  | Vincent Lecours and Michael Espriella <br> [Can multiscale roughness help computer-assisted identification of coastal habitats in Florida?](https://doi.org/10.30437/geomorphometry2020_24) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Lecours.pdf) <br> [video](https://youtu.be/zx19j3qqCts) |
|16.00-16.15  | Charles Holderman, Steve Kopp and Nawajish Noman <br> [A New Analytic Framework and Notebook for Terrain Analysis](https://doi.org/10.5281/zenodo.5297224) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Kopp.pdf)  <br> [video](https://youtu.be/M7CsJ8eagc0) |
|16.30-16.45  | Discussion and Conclusion|


### SEPTEMBER 14 DYNAMICS OF EARTH SURFACE: AUTOMATED SURFACE ANALYSIS AND MODELIZATION

|10.00:      | Opening connections|
|10.30-10.45 | Peter Guth <br> [Using high-resolution lidar point clouds to evaluate 1-3 arc second global digital elevation models](https://doi.org/10.30437/GEOMORPHOMETRY2020_31) <br>[presentation](https://zenodo.org/record/5504441) <br> [video](https://youtu.be/K3I81m_2jxE) |
|10.45-11.00 | Tera Geoffroy and Peter Guth <br> [Using high-resolution ICESat-2 point clouds to evaluate 1-3 arc second global digital elevation models](https://doi.org/10.30437/GEOMORPHOMETRY2020_29)<br> [published as full paper in Transactions in GIS](https://doi.org/10.1111/tgis.12825)  <br> [presentation](https://zenodo.org/record/5504446) <br> [video](https://youtu.be/I1B27IjT0zI) |
|11.00-11.15 | Daniele Pinton, Alberto Canestrellli, Christine Angelini, Benjamin Wilkinson, Peter Ifju and Andrew Ortega <br> [Estimating the spatial distribution of vegetation height and ground level elevation in a mesotidal salt marsh from UAV LiDAR derived point cloud](https://doi.org/10.30437/GEOMORPHOMETRY2020_33) <br> [published as full paper in Earth Surface Processes and Landforms](https://doi.org/10.1002/esp.4992) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Pinton.pdf)  <br> [video](https://youtu.be/GV78NRpRhyg) |
|11.15-11.30 | Guanghui Hu, Liyang Xiong and Guoan Tang <br> [Mathematical vector framework for land surface curvature calculation from triangulated irregular network](https://doi.org/10.30437/GEOMORPHOMETRY2020_12) <br> [video](https://youtu.be/sfkXCwu1lm4) |
|11.30-11.45 | Break time |
|11:45-11:50 | Announcement of [Lifetime Achievement Award](https://zenodo.org/record/5504437) <br> [video](https://youtu.be/PrrKBZxCoao) |
|11.50-12.20 | **Keynote talk: Michael Hutchinson**  <br>  Reflections on adding the Z dimension to earth system analysis <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Hutchinson.pdf) <br> [video](https://youtu.be/fHwtiDl7Vik) |
|12.20-12.35 | Sebastiano Trevisani <br> [Geomorphometric features selection based on intrinsic dimension estimation](https://doi.org/10.30437/GEOMORPHOMETRY2020_11) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Trevisani.pdf) <br> [video](https://youtu.be/EmJLkzTh7g4) |
|12.35-12.50 | Kacper Jancewicz, Piotr Migoń, WioletaPorębna and Milena Różycka <br> [High-resolution geomorphometry – a tool for better understanding the genesis and contemporary processes in erosional sandstone landscapes](https://doi.org/10.30437/GEOMORPHOMETRY2020_32 )<br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Jancewicz.pdf) <br> [video](https://youtu.be/Yyd1TMzLCN0) |
|12.50-13.00 | Discussion and Conclusion|
|13.00-14.00 | Lunch time|
|14.00-14.15 | Tomislav Hengl and Leandro Parente <br> Continental-scale Digital Terrain Model for EU based on Ensemble Machine Learning <br> [video](https://youtu.be/6dD6-eCXaXA) |
|14.15-14.30 | Gaurav Sinha and Samantha Arundel <br> [Automated Extraction of Areal Extents For GNIS Summit Features Using the Eminence-Core Method](https://doi.org/10.30437/GEOMORPHOMETRY2020_10) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Sinha.pdf) <br> [video](https://youtu.be/wzLPM8mstxw) |
|14.30-14.45 | Olga Ishalina, Dmitrii Bliakharskii and Igor Florinsky <br> [Detection of crevasses using high-resolution digital elevation models: Comparison of geomorphometric modeling and texture analysis](https://doi.org/10.30437/GEOMORPHOMETRY2020_3) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Ishalina.pdf) <br> [published as full paper in Transactions in GIS](https://doi.org/10.1111/tgis.12790) | 
|14.45-15.00 | Carlos Grohmann, Guilherme Garcia, Alynne Affonso and Rafael Albuquerque <br> [Coastal dune modelling from airborne LiDAR, terrestrial LiDAR and Structure from Motion–Multi View Stereo](https://doi.org/10.30437/GEOMORPHOMETRY2020_30) <br> published as https://doi.org/10.1016/j.cageo.2020.104569 <br> [published as full paper in Computers & Geosciences](https://doi.org/10.1016/j.cageo.2020.104569) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Grohmann.pdf)  <br> [video](https://youtu.be/zVo80-RuvgE) |
|15.00-15.15 | Break time|
|15.15-15.30 | Bartłomiej Szypuła <br>[DEM from topographic maps - as good as DEM from LiDAR?](https://doi.org/10.30437/GEOMORPHOMETRY2020_34) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Szypula.pdf) <br> [video](https://youtu.be/gOdUMg_G7Bs) |
|15.30-15.45 | Anna Dedkova,Igor Florinsky and Nikolay Djuzhev <br> [Analysis of topography of silicon wafers and wafer-based structures by geomorphometric modeling](http://dx.doi.org/10.5281/zenodo.5295613) <br> [video](https://youtu.be/tML5FSgRieA) |
|15.45-16.00 | Peter L. Guth and Morgan E. Kane <br> [Evaluation of slopes calculated from TanDEM-X digital elevation models at 3 spatial resolutions](https://doi.org/10.5281/zenodo.5260534) <br> [video](https://youtu.be/z8B_kbCt7zg) |
|16.00-16.15 | Ivan Marić, Ante Šiljeg, Fran Domazetović and Neven Cukrov <br> [A framework for using handheld 3D surface scanners in quantifying the volumetric tufa growth](https://zenodo.org/record/5484684) <br> [presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Maric.pdf) |
|16.15-16.30 | Ante Šiljeg, Vlatko Roland, Lovre Panđa, Ivan Marić, Fran Domazetović, Silvija Šiljeg and Rina Milošević <br> [Development of the new methodological framework for multiscale modeling of urban pluvial flooding](https://zenodo.org/record/5336065) <br> [presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Siljeg.pdf) <br> [video](https://youtu.be/SmHDxO2fKIQ) |
|16.30-16.45 | Discussion and conclusion|


### SEPTEMBER 15 MODELING GEOMORPHOLOGICAL PROCESSES

|10.00: Opening connections|
|10.15: Conference opening|
|10.30-10.45 | Andrei Dornik, Lucian Drăguț, Marinela Adriana Chețan, Takashi Oguchi, Yuichi Hayakawa and Mihai Micu <br> [Towards a consistent set of land-surface variables for landslide modelling](https://doi.org/10.30437/GEOMORPHOMETRY2020_44) <br> [presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Dornik.pdf)<br> [video](https://youtu.be/ix4mXf7sV38) |
|10.45-11.00 | Mihai Niculita <br> [Landslide topographic signature prediction using segmentation of roughness and Random Forest](https://doi.org/10.30437/GEOMORPHOMETRY2020_48) <br> [video](https://youtu.be/COacJlZYSX0) |
|11.00-11.15 | Stefan Steger <br> [The role of pre-landslide morphology in statistical modelling of landslide-prone areas](https://doi.org/10.30437/GEOMORPHOMETRY2020_51) <br> [presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Steger.pdf)<br> [published as full paper in Geomorphology](https://doi.org/10.1016/j.geomorph.2020.107041) |
|11.15-11.30 | Mio Kasai <br> [Incorporating ground cracks in the estimation of post-seismic landslide susceptibility](https://doi.org/10.30437/GEOMORPHOMETRY2020_45) <br> [published as full paper in Transactions in GIS](https://doi.org/10.1111/tgis.12900)  <br> [presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Kasai.pdf)  <br> [video](https://youtu.be/U_X-VXpMSHk) |
|11.30-11.45 | Break time|
|11.45-12.15 | Igor Florinsky, Sergey Filippov and Alexander Govorov <br> [3D marine geomorphometry for the Arctic Ocean](https://doi.org/10.30437/GEOMORPHOMETRY2020_22) <br> [video](https://youtu.be/tH3OcFpEvTk) |
|12.15-12.30 | Margaret Dolan, Lilja Bjarnadóttir, Terje Thorsnes, Markus Diesing and Shyam Chand <br> [Geomorphometry in the deep Norwegian Sea](https://doi.org/10.30437/GEOMORPHOMETRY2020_20) <br> [presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Dolan.pdf)<br> [video](https://youtu.be/dvjan-SSojA) |
|12.30-12.45 | Queralt Guerrero, Ariadna Salabarnada, Amadeu Deu and Marcelo Devincenzi <br> [Marine geophysical investigations for offshore wind farms and submarine interconnection cables](https://zenodo.org/record/5354500) <br> [presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Guerrero.pdf)<br> [video](https://youtu.be/yvNfoEQ9lFo) |
|12.45-13.30 | **Meeting of the International Society for Geomorphometry.** Everybody is welcome to attend|
|13.00-14.00 | Lunch time|
|14.00-14.15| Ivica Milevski, Marjan Temovski, Balazs Madarasz, Zoltan Kern and Zsofia Ruszkiczay-Rudiger <br> [Geomorphometry of the cirques of Shar Mountain](https://doi.org/10.30437/GEOMORPHOMETRY2020_25) <br> [presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Milevski1.pdf)<br> [video](https://youtu.be/5wWXmnwvdgc) |
|14.15-14.30 | Ivica Milevski, Bojana Aleksova and Sonja Lepitkova <br> [Geomorphometric characteristics of the high mountains in North Macedonia](https://doi.org/10.30437/GEOMORPHOMETRY2020_41) <br> [presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Milevski2.pdf)<br> [video](https://youtu.be/0_gvl1Go88w) |
|14.30-14.45 | Ian Sylvester Evans, Nicholas J. Cox,Mihai Niculita and David Milledge <br> [Hypsoclinometric evidence of the degree of modification of mountains by glacial erosion](https://doi.org/10.30437/GEOMORPHOMETRY2020_21) <br> [presentation](https://zenodo.org/record/5502181) <br> [video](https://youtu.be/8ea8cGJppm8) |
|14.45-15.00 | Simone Tarquini, Massimiliano Favalli, Melissa Pfeffer, Mattia De' Michieli Vitturi, Sara Barsotti and Gro Pedersen <br> [Assessing the impact of lava flows during the unrest of Svartsengi volcano in the Reykjaness peninsula, Iceland](https://doi.org/10.30437/GEOMORPHOMETRY2020_52) |
|15.15-15.30 | Giuseppe Amatulli, Tushar Sethi, Longzhu Shen, Jaime Ricardo, Garcia-Márquez, Jens Kiesel and Sami Domisch <br> [A new and extendable global watershed and stream network delineation using GRASS-GIS](https://doi.org/10.30437/GEOMORPHOMETRY2020_55) <br> [presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Amatulli.pdf) <br> [video](https://youtu.be/TK3oyZhURto) |
|15.30-15.45 | Atrayee Biswas, Sunando Bandyopadhyay and Abhijit Chakraborty <br> [Characterizing Gully Morphology using Structure-from-Motion (SfM) in Garhbeta Badlands, West Bengal, India](https://zenodo.org/record/5336981) <br> [video](https://youtu.be/ZAeOMwKLlE0) |
|15.45-16.00 | Badal Pokharel, Massimiliano Alvioli and Samsung Lim <br> [Relevance of morphometric parameters and completeness of inventories in susceptibility modelling of earthquake-induced landslides](https://doi.org/10.30437/GEOMORPHOMETRY2020_49) <br>[published as full paper in Scientific Reports](https://doi.org/10.1038/s41598-021-00780-y) <br> [presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Pokharel.pdf)  <br> [video](https://youtu.be/KDVK-lZAOZU) |
|16.00-16.15 | Massimiliano Alvioli, Michele Santangelo, Federica Fiorucci, Mauro Cardinali, Ivan Marchesini, Paola Reichenbach and Mauro Rossi <br> [A data-driven method for assessing the probability for terrain grid cells of initiating rockfalls on a large area](https://doi.org/10.30437/GEOMORPHOMETRY2020_43)<br> [published as full paper in Engineering Geology](https://doi.org/10.1016/j.enggeo.2021.106301) <br> [presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Fiorucci.pdf) <br> [video](https://youtu.be/vsqZmaaP9zc) |
|16.15-16.30 | Nada Ait Ayad, Adnane Habib, Khalid Elkhalidi, Abdeloihab Choukri and Abdelmounim Charif <br> [Geomorphometric Analysis for Mapping Platforms of the Mazagan Corridor, Morocco](https://zenodo.org/record/5346585) | 
|16:30-16:45 | Announcement of best paper and best student paper awards recipients |
|            | **Best student paper award**
|            | **Daniele Pinton**, Alberto Canestrellli, Christine Angelini, Benjamin Wilkinson, Peter Ifju and Andrew Ortega <br> [Estimating the spatial distribution of vegetation height and ground level elevation in a mesotidal salt marsh from UAV LiDAR derived point cloud](https://doi.org/10.30437/GEOMORPHOMETRY2020_33) <br> published as [full paper in Earth Surface Processes and Landforms](https://doi.org/10.1002/esp.4992) <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Pinton.pdf)  <br> [video](https://youtu.be/GV78NRpRhyg) |
|            | **Best paper award #1**
|            | Michael Hutchinson  <br>  Reflections on adding the Z dimension to earth system analysis <br>[presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Hutchinson.pdf) <br> [video](https://youtu.be/fHwtiDl7Vik) |
|            | **Best paper award #2**
|            | Massimiliano Alvioli, Michele Santangelo, **Federica Fiorucci**, Mauro Cardinali, Ivan Marchesini, Paola Reichenbach and Mauro Rossi <br> [A data-driven method for assessing the probability for terrain grid cells of initiating rockfalls on a large area](https://doi.org/10.30437/GEOMORPHOMETRY2020_43)<br> [published as full paper in Engineering Geology](https://doi.org/10.1016/j.enggeo.2021.106301) <br> [presentation]({{site.baseurl}}/uploads/pdf/pdf2021/Fiorucci.pdf) <br> [video](https://youtu.be/vsqZmaaP9zc) |
|16.30-17.00 | Discussion and closing remaks|

