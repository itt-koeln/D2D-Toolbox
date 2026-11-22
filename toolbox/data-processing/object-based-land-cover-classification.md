---
layout: default
title: "Object-based land cover classification"
parent: Data Processing
grand_parent: D2D Toolbox
nav_order: 11
permalink: /toolbox/data-processing/object-based-land-cover-classification/
---

# Object-based land cover classification

*Posted 2018-06-18* · Category: Geoprocessing

**Prepared by: Pedro Ivo Bastos de Castro**

![]({{ site.baseurl }}/assets/uploads/2018_06_spring.gif)

---

**1. Background**

The ability to extract reliable land cover information from satellite sensors allow the natural resources monitoring and provide essential inputs for integrated water resources management.

One important software for Land use land cover classification is Spring. More than a classification tool, Spring encompasses representation of raster and vector files in a single environment and contains a set of standard digital image processing functions.

Moreover, the software offers the possibility of working with an Object-based Image Analysis (OBIA), which provides significant advantages in land cover classification.

---

**2. Principle**

The OBIA consists in transforming a complex and heterogeneous satellite image in a layer containing image objects. Its internal homogeneity and external contrast characterize these objects. The procedure of turning a complex image in image-objects is known as segmentation process. Once the image is converted into distinct homogeneous regions, a sampling process is started. The sampling aims to provide information regarding the spectral patterns of different land surface classes, which are user-defined.  Finally, the classification method Bhattacharya is performed.

---

**3. Manual**

First decision has to be made before starting the classification:

- Classes to be mapped
- Scale (spatial resolution)
- Minimum accuracy in the automatic process (it will define the amount of time for further manual editing process)

The required inputs for land use Land cover Classification are:

- Multi-spectral Image (Landsat, MODIS, Sentinel, etc.)
- Training samples (can be obtained in the field or via visual interpretation in Spring environment)

•    Validation samples (can be obtained in the field or via visual interpretation in Spring environment)

---

**4. Exercise**

The exercises are included in the E-learning Unit for Land Use Land Cover Classification using Spring in the following [link](https://th-koeln.sciebo.de/s/iG1ZvNuipCtpI3E)

---

**5. Example**

Carriello, F. Rezende, F.S., Neves, O.M.S.  Rodriguez, D.A. 2016. Forestry expansion during the last decades in the Paraiba do Sul basin – Brazil. The International Archives of the Photogrammetry, Remote Sensing and Spatial Information Sciences, Volume XLI-B8.
