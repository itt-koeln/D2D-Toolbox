---
layout: tool
title: "Supervised Land cover classification in QGIS"
parent: Data Processing
grand_parent: D2D Toolbox
nav_order: 18
permalink: /toolbox/data-processing/supervised-land-cover-classification-in-qgis/
summary: "Guide to supervised land cover classification of satellite imagery in QGIS, with background, principles, and a step-by-step exercise."
authors: "Abdrahman A.; Kamara A.B.; Cubillos N.; Mengen D.; Wolde S.G"
year: "2019"
kind: training
topics: ["Geoprocessing"]
software: ["QGIS"]
keywords: ["land cover", "supervised classification", "satellite imagery", "remote sensing"]
---

*Posted 2019-05-28* · Category: Geoprocessing

![]({{ site.baseurl }}/assets/uploads/2019_05_qgis.png)

## Background

Land use and land cover greatly represent the integrating elements of natural resources base. Changes in land cover and land use affect the global systems which include atmosphere, climate, and sea level or they occur in a localized fashion in enough places to add up to a significant total (Meyer and Turner, 1992).

Land cover is a geographical feature which may form a reference base for applications ranging from forest and rangeland monitoring, production of statistics, planning, investment, biodiversity, climate change, to desertification control. In addition to a high demand for improved land cover datasets because of an increasing need to be able to precisely describe and classify land cover in order to develop sustainable land use systems, there is also a growing need for standardization and compatibility between data sets and for the possibility to map, evaluate and monitor wide areas.

Unlike other tools for land classification (e.g. Semi-automatic plugins in Q GIS), the unsupervised classification in R is most commonly used when there is no prior knowledge of the study area.

## Principle

Supervised classification uses the technique of analyzing satellite images based on relating each spectral domain to a specific land use i.e. a supervised creator will select random pixel samples in an image to relate it to a unique land use class, then those selected pixels will be reflected on other pixels that carry similar or closer values.

Supervised Classification also semi-automatic classification is an image processing technique that allows for the identification of materials in an image, according to their spectral signatures. There are several kinds of classification algorithms, but the general purpose is to produce a thematic map of the land cover.

## Manual

QGIS is an open source Geographic information system software that can be downloaded from [here](https://qgis.org/en/site/forusers/download.html).

QGIS provides several functions and enhancements. You can view, manage, edit, analyze data and create print-ready maps.

You can also download QGIS [manuals and user guides](https://www.qgis.org/de/docs/index.html) for more information on the software.

## Exercise and Example

Step by step exercise with an example for downloading satellite images from USGS earth explorer and land use classification in QGIS can be found in the [Supervised land classification guide]({{ site.baseurl }}/assets/uploads/2019_05_supervisedlandclassificationguide.pdf) (page 1 - 70).
