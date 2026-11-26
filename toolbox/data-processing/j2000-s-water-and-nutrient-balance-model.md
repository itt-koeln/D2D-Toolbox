---
layout: tool
title: "J2000-S (water and nutrient balance model)"
parent: Data Processing
grand_parent: D2D Toolbox
nav_order: 7
permalink: /toolbox/data-processing/j2000-s-water-and-nutrient-balance-model/
summary: "Physically-based, fully distributed hydrological model with nutrient transport routines combining J2000 and SWAT, run in the JAMS framework."
authors: "Santiago Penedo"
year: "2018"
kind: method
topics: ["Rainfall-Runoff modelling"]
software: ["JAMS"]
keywords: ["rainfall-runoff", "water balance", "nutrient transport", "hydrological response units"]
---

*Posted 2018-06-18* · Category: Rainfall-Runoff modelling

## Background

J2000 is a physically-based and fully distributed hydrological model developed by Krause (2001) to understand and describe the hydrological processes taking place at the basin level. J2000 was designed for dynamic simulations of water transport in meso- to macro-scale river basins (Krause 2001).

Fink et al. (2007) worked on the enhancement of the J2000 into the J2000-S model to widen the scope of hydrological simulation to the area of water quality. J2000-S is a further development of the J2000 model combined with nutrient transport routines of the semi-distributive Soil and Water Assessment Tool (SWAT; Arnold et al. 1998).

The models work within the Java-based modeling framework JAMS (Jena Adaptable Modeling System; Kralisch & Krause 2006; Kralisch et al. 2007). The modular and object-oriented structure of the modeling system allows a customized selection or adaptation of the components, like for example the choice between different evapotranspiration equations or modifications depending on data availability and modelling approach.

## Principle

The water pathways are calculated on the basis of the Hydrological Response Units (HRUs). The HRU concept was first proposed by Leavesley et al. (1983) based on homogeneous topological modeling entities. Later, the concept was revisited by Flügel (1996) suggesting HRUs as distributive heterogeneously units with homogeneous land use and pedotopogeological characteristics controlling water dynamics. The latter spatial distribution concept of HRUs provides the possibility to simulate land use changes, even on the field scale and was, therefore, included in the J2000 model.

JAMS/J2000-S is a flexible modular process-oriented modelling system. Being possible to select only those process modules required to represent the river basin. For instance, here some examples of routines present in the model are listed:

1. Hydrological routines
   - Climate data regionalization
   - Meteorological data correction
   - Evapotranspiration
   - Radiation
   - Interception
   - Soil
   - Groundwater
   - Routing
2. Nitrogen related routines
   - Plant growth
   - Soil temperature
   - Soil nitrogen
   - Land-use management

As it can be seen the J2000 has different modules representing hydrological processes such as evapotranspiration, snow accumulation, and melt, infiltration, interception, groundwater and reach routing. Based on these processes, the J2000 generates four different runoff components (which can be seen in Figure 6‑1): (i) RD1 which is the fast direct runoff flowing over the surface, (ii) RD2 which is the slow direct runoff (also known as interflow 1) which can be regarded as a lateral subsurface flow (Nepal 2012), (iii) RG1 which is the “fast” baseflow component (also known as interflow 2) originating in the upper part of the aquifer, (iv) RG2 which is the “slow” baseflow component originating in the bottom part of the aquifer.

The following image depicts the main routines and their interaction with the J2000-S model:

![]({{ site.baseurl }}/assets/uploads/2018_06_j2000-530x334.png)

## Manual

A wiki is available online explaining the routines and their mathematical equations, data format and basic information to run the model ([here](http://jams.uni-jena.de/ilmswiki/index.php/Water_and_Nutrient_Balance_Model_J2000-S)).

## Example

Fink et al. (2007) published a paper on the development and application of the model in the context of the EU Water Framework Directive ([here](https://www.adv-geosci.net/11/123/2007/)).
