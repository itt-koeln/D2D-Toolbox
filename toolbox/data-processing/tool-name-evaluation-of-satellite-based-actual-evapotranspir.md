---
layout: tool
title: "Evaluation of Satellite-Based Actual Evapotranspiration Products"
parent: Data Processing
grand_parent: D2D Toolbox
nav_order: 19
permalink: /toolbox/data-processing/tool-name-evaluation-of-satellite-based-actual-evapotranspir/
summary: "Evaluates satellite-based actual evapotranspiration products by comparing them with prior studies and integrated NDVI, using land cover to isolate agricultural areas."
authors: "Saher Ayyad"
year: "2019"
kind: method
topics: ["Crop water requirement"]
software: ["ArcGIS"]
keywords: ["actual evapotranspiration", "remote sensing", "integrated NDVI", "crop water requirement"]
---

*Posted 2019-05-28* · Category: Crop water requirement

## Background

Water scarcity has become a limiting factor for agriculture, especially in arid and semi-arid regions, where crop water consumption exceeds precipitation and irrigation water from surface or groundwater resources is needed to compensate for the deficit. Due to the lack of field measurements for actual crop water use in data-scarce regions, remote sensing (RS) data are of vital significance for providing spatio-temporal information on the actual evapotranspiration (ETa).

## Principle

Following the success of open access rainfall products based on earth observation data, nowadays the actual evapotranpiration algorithms are implemented in satellite-based open access products that are supported by several providers. These ETa products can be analyzed directly to estimate the actual crop water demand in different scales.

## Manual

This tool develops a process to evaluate the performance of these RS ETa products as follow:

- Using the available previous RS ETa studies in the same region, preferably the studies that used some ground-truth data for validation. Additionally,
- Using the direct relationship between the ETa and the integrated Normalized Difference Vegetation Index (iNDVI) to assess the ETa estimates from different ETa products. The greater the iNDVI the higher the ETa. This correlation could be done on a seasonal or annual basis.

In order to estimate the ETa over the agricultural areas, there is a need for high temporal resolution Land Cover images to capture the agricultural areas and their spatial-temporal distribution. Several Landcover products can be found in the ITT toolbox- Public Domain Data).

ArcGIS software is the main used tool for the whole process.

## Example

Al Zayed, I.S., Elagib, N.A., Ribbe, L., Heinrich, J., 2016. Satellite-based evapotranspiration over Gezira Irrigation Scheme, Sudan: A comparative study. Agric. Water Manag. 177, 66–76. https://doi.org/10.1016/j.agwat.2016.06.027
