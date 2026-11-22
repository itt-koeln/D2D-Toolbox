---
layout: default
title: "Unsupervised Land cover classification in R"
parent: Data Processing
grand_parent: D2D Toolbox
nav_order: 20
permalink: /toolbox/data-processing/unsupervised-land-cover-classification-in-r/
---

# Unsupervised Land cover classification in R

*Posted 2019-05-28* · Category: Geoprocessing

**Prepared by: Abdrahman A.; Kamara A.B.; Cubillos N.; Mengen D. and Wolde S.G                                                                                        ![]({{ site.baseurl }}/assets/uploads/2019_05_rlogo.jpg)**

---

**1. Background**

Land use and land cover greatly represent the integrating elements of natural resources base. Changes in land cover and land use affect the global systems which include atmosphere, climate, and sea level or they occur in a localized fashion in enough places to add up to a significant total (Meyer and Turner, 1992).

Land cover is a geographical feature which may form a reference base for applications ranging from forest and rangeland monitoring, production of statistics, planning, investment, biodiversity, climate change, to desertification control. In addition to a high demand for improved land cover data sets because of an increasing need to be able to precisely describe and classify land cover in order to develop sustainable land use systems, there is also a growing need for standardization and compatibility between data sets and for the possibility to map, evaluate and monitor wide areas.

Unlike other tools for land classification (eg. Semi-automatic plugins in Q GIS), the unsupervised classification in R is most commonly used when there is no prior knowledge of the study area.

---

**2. Principle**

The algorithm combines pixels with similar spectral characteristics into unique groups/classes/clusters with respect to some statistically determined conditions (e.g. minimizing mean square root error within each cluster)

When compared to supervised classification technique, unsupervised classification normally requires initial input from the analyst. Groupings of spectral information present in pixels are examined in the multispectral feature space. Unlike supervised classification, unsupervised classification requires the collection of no training data and the program is allowed to select the class mean and covariance matrices which will be further used for classification.

---

**3. Manual**

R is an open source programming language that can be downloaded from [here](https://cran.r-project.org/mirrors.html) which uses R-Studio as its integrated development environment (IDLE) which can also be downloaded from [here](https://www.rstudio.com/products/rstudio/download/)
This software makes use of numerous free packages that can be downloaded and imported into either the script or console window of R Studio. For the purpose of land cover classification, geo-processing packages (eg. raster, rgdal, rstoolbox, RColorBrewer) can be installed and called using ‘install’ and ‘import’  respectively.

You can also download R [manuals](https://cran.r-project.org/manuals.html) for more information on the software.

---

**4. Exercise**

Step by step exercise for downloading and running the commands can be found in the [attachment]({{ site.baseurl }}/assets/uploads/2019_05_stepbystepunsupervisedclassificationinr.pdf)  (page 1 through 15).

---

**5. Example**

An example of the application of the tool with detailed code and description can also be found in [attachment]({{ site.baseurl }}/assets/uploads/2019_05_stepbystepunsupervisedclassificationinr.pdf) (page 16 to 17).
