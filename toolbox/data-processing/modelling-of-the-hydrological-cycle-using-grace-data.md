---
layout: tool
title: "Modelling of the hydrological cycle using GRACE data"
parent: Data Processing
grand_parent: D2D Toolbox
nav_order: 10
permalink: /toolbox/data-processing/modelling-of-the-hydrological-cycle-using-grace-data/
summary: "Guide and manuals for using GRACE satellite gravity data to model terrestrial water storage changes, including R-based download and Nile Basin case study."
authors: "Ali Zomorodian, Ian McNamara, Oscar M. Baez Villanueva"
year: "2021"
kind: training
topics: ["Modeling of hydrological cycle"]
software: ["R"]
keywords: ["GRACE", "terrestrial water storage", "gravity recovery", "hydrological cycle"]
---

*Posted 2021-09-28* · Category: Modeling of hydrological cycle

## Background

The Gravity Recovery And Climate Experiment (GRACE) space mission is an international collaboration between the National Aeronautics and Space Administration (NASA) and the Deutsche Forschungsanstalt für Luft und Raumfahrt (DLR). This project aims to provide high-resolution, accurate, global data about both mean and time-variable components of Earth’s gravity field, which can be used to monitor changes in water storage and snow in the continents, particularly in areas where measuring stations are sparsely distributed.

## Principle

The GRACE mission consists of two identical co-orbiting satellites (GRACE-1 and GRACE-2) that follow each other, separated by a distance ranging from 170 to 270 km. They form an instrument that measures the abnormalities of the Earth’s gravity field by measuring the relative distance between the center of mass of the two satellites via a microwave tracking system. This can be used to determine changes in terrestrial water storage.

For a detailed overview of how the satellite measurements are transformed into estimates of measurements of terrestrial water storage anomalies as well as an overview of the data products available to the public, see the **[How GRACE Works]({{ site.baseurl }}/assets/uploads/2021_09_howgraceworks.pdf)** report.

## Manual

We have developed two documents on how to use GRACE data.

- The first document ([Automatic Downloading of GRACE Products Using R]({{ site.baseurl }}/assets/uploads/2021_09_automaticdownloadingofgraceproductsusingr.pdf)) instructs the user how to download GRACE Level-3 data using the R Project for Statistical Computing.

The second document ([Multi-Annual Analysis of TWS Using GRACE (Nile Case Study)]({{ site.baseurl }}/assets/uploads/2021_09_multiannualanalysisoftwsusinggracenilecasestudy.pdf)) shows an example of how to use GRACE Level-3 data to derive a time series of changes in TWS over the Nile Basin.

## Exercise and Example

Exercise: None

Example: [Rodell et al. (2018): Emerging trends in global freshwater availability](https://www.nature.com/articles/s41586-018-0123-1)
