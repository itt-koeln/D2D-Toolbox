---
layout: default
title: "Satellite Rainfall Estimates analysis"
parent: Data Analysis
grand_parent: D2D Toolbox
nav_order: 4
permalink: /toolbox/data-analysis/satellite-rainfall-estimates-analysis/
---

# Satellite Rainfall Estimates analysis

*Posted 2018-06-18* · Category: SREs and DEM validation tools

**Prepared by: Oscar Baez**

![]({{ site.baseurl }}/assets/uploads/2019_05_rlogo.jpg)

---

**1. Background**

Precipitation is one of the key parameters of the water cycle. However, in scarce data regions, the correct representation of rainfall is severely limited. The technological development has led to new sources of information such as the satellite rainfall estimates (SREs). The SREs are global or regional precipitation estimates that are calculated based on infrared or microwave sensors installed on geostationary (GEO) and low-earth orbit (LEO) satellites respectively. The temporal resolution can be hourly, daily or monthly and the spatial resolution is represented by pixels of different size depending on the product (generally from 0.05° to 0.25°, approximately from 5km to 25 km near the equator).

Moreover, the SREs can perform differently over diverse environments and currently, there is no best performing SRE for the entire world. Therefore, a validation process must be performed in order to determine the satellite estimate that better represents the studied area.

In order to handle the large data of the SREs and to compare them in order to select the best performing one over a certain area, the R-Project for statistical computing will be used (more information [here](https://www.r-project.org/)).

---

**2. Principle**

A point-to-pixel analysis is a comparison between the observed data in a certain rain gauge station and the pixel of the SRE that contains it. There are different indices to assess the performance of the SREs. Here, the modified Kling-Gupta Efficiency (KGE´) and the Root Mean Squared Error (RMSE) will be used to evaluate different rain gauge stations in order to determine the best performing SRE over an area.

---

**3. Manual**

The open-source R software can be downloaded from [here](https://cran.r-project.org/mirrors.html) and RStudio, which is an integrated development environment (IDE) for R can be downloaded [here](https://www.rstudio.com/products/rstudio/download/).

Different manuals for R can be found [here](https://cran.r-project.org/manuals.html).

The specific manuals for SREs analysis can be found in the attachment from the following [link](https://th-koeln.sciebo.de/s/qpt7wfE7MF5sb6A) as part of a developed Learning Unit of satellite rainfall estimates (SREs).

---

**4. Exercise**

An exercise of a point-to-pixel analysis can be also found also in the attachment in the previous link in the Manual section.

---

**5. Example**

Zambrano et al., (2017) evaluated the Chilean country with a point-to-pixel methodology ([Temporal and spatial evaluation of satellite-based rainfall estimates across the complex topographical and climatic gradients of Chile](https://www.hydrol-earth-syst-sci.net/21/1295/2017/hess-21-1295-2017.pdf)).
