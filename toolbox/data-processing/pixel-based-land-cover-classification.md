---
layout: default
title: "Pixel-based land cover classification"
parent: Data Processing
grand_parent: D2D Toolbox
nav_order: 12
permalink: /toolbox/data-processing/pixel-based-land-cover-classification/
---

# Pixel-based land cover classification

*Posted 2018-06-18* · Category: Geoprocessing

**Prepared by: Pedro Ivo Bastos de Castro                                ![]({{ site.baseurl }}/assets/uploads/2018_06_r.png)**

---

**1. Background**

The Satellite-based land cover Classification with R currently developed in ITT is based on the RStoolbox package, which encompasses a set of function for performing standard remote sensing tasks. For example, the packages allow you to read Landsat products through its metadata, apply DN – physical values conversion, masking, generate spectral indices, PCA, Tasseled-cap Transformations, unsupervised, and supervised classification. For the latter, you will need the software QGis additionally for collecting the training and validation samples.

The RStoolbox package relies on some other primary packages such as raster and rgdal. Commonly, those dependencies are installed when you run the install function for the RStoolbox.

---

**2. Principle**

The methodology uses the patterns of spectral response from surface features detected by multispectral sensors onboard satellites. It is based on concepts related to the wave theory. The model is established by taking into account the spectral signature of surface targets, such as water, vegetation, bare soil, and edifications. Commonly, the multispectral bands used for the land use classification model range from visible to infrared. The classification is performed at the pixel level.

---

**3. Manual**

First, you need to install the software R (visit: <https://www.r-project.org/>). It is recommended to download the R Studio (in <https://www.rstudio.com/products/rstudio/download/>), which will provide you syntax-highlighting editor to supports code execution. After installing both R software and RStudio, you will need to apply the basic commands to install the package and start working.

To install those packages, you need to run the command:

install.packages(“RStoolbox”)

Afterward, you need to load the library with the following command:

Library(RStoolbox)

Note: When asked for installing the dependencies, say yes.

---

**4. Exercise**

A step by step for land cover classification using R is provided as an attachment.

For the guided exercises in the reference book, check the following link:
<http://book.ecosens.org/data/>

---

**5. Example**

Martin Wegmann, Benjamin Leutner, and Stefan Dech. Remote Sensing and GIS for Ecologists. Pelagic Publishing. 2016.

---

The document can be downloaded from here: [toolbox description\_landcover\_bastosdecastro]({{ site.baseurl }}/assets/uploads/2018_06_toolboxdescription_landcover_bastosdecastro.docx)
