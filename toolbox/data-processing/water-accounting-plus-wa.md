---
layout: tool
title: "Water Accounting Plus (WA+)"
parent: Data Processing
grand_parent: D2D Toolbox
nav_order: 21
permalink: /toolbox/data-processing/water-accounting-plus-wa/
summary: "Describes the Water Accounting Plus (WA+) framework for tracking water depletion and flows in a basin using remote sensing data and standardized sheets."
authors: "Muhammad Khalifa"
year: "2018"
kind: training
topics: ["Water accounting"]
software: ["ArcGIS", "QGIS", "Excel"]
keywords: ["water accounting", "water balance", "remote sensing", "evapotranspiration"]
---

*Posted 2018-06-18* · Category: Water accounting

![]({{ site.baseurl }}/assets/uploads/2018_06_wateraccounting.png)

## Background

Resources are highly needed to be managed in an integrated way since it involves different disciplines (Medema et. al., 2008). Standardization of water resources reporting is of high importance to effectively manage this vital resource (Karimi et. al, 2013a). Several attempts have been carried out to standardize water reporting in frameworks that could be easily understood by different stakeholders. Examples of these frameworks include System of Environmental-Economic Accounting for Water (SEEAW), FAO's Aquastat, and the Water Accounting Standard of Australia. WA approach was developed by David Meldon from the International Water Management Institute (IWMI) (Meldon, 1997). It built on the earlier works of Meldon, 1997, Perry, 2007, Foster and Perry, 2010, and Perry and Bucknall, 2009. The ultimate goal of the WA is to "track inflows, assets, liabilities, stocks, and reserves for a particular area over a period of time" (Karimi et. al., 2013a, p. 1). Water Accounting (WA+) is a development of the IWMI approach and proposed by Karimi et. al., 2013a. It differs from the original approach in that instead of dealing with withdrawals, it tracks water depletion. In addition, it could be conducted using public domain remote sensing data, which offers a way for a standardized and transparent framework for data collection (Karimi et. al., 2013a). It incorporates data from public domain remote sensing sources (e.g. P from TRRM, ET from MODIS16) to produce the WA+ sheets. To assess the water different aspects of the water resources in a system, several indicators could be calculated based on the data collected in the four WA+ sheets.

## Principle

Water Accounting (WA) approach uses the principles of the traditional hydrological water balance, which describes the water moving in and out of a system. In Integrated Water Resources Management approach the basin is considered as the practical hydrological unit for managing water (GWP, 2009). In water balance, different components are included. The simple expression of this concept in a watershed or a water basin level is understood by parameters such as precipitation, evapotranspiration, runoff and storage change. This is represented by the water balance equation (Zhang et.al., 2002): ΔS= P – ET - Q - R, where ΔS is the change in storage in soil, P is precipitation, Q is the runoff, ET is the evapotranspiration and R is the average catchment recharge. The classical approach of estimating the water balance is by using ground-based measurement for these parameters (Oki et. al., 1995).

Recently with the availability of remote sensing data and development techniques, estimating water balance by using these data and these techniques become more popular (Mekonnen, 1998). This is because remote sensing data provide a spatial coverage that is not feasible by the traditional approach. The major advantage of such approach is that water balance could be estimated for areas with limited or no ground-based data. An example of this advantage is estimating of the water balance for Lake Manyara in Tanzania (Deus et. al., 2013). During the last years, many studies were conducted around the world to utilize remote sensing data in estimating water balance).

![]({{ site.baseurl }}/assets/uploads/2018_06_wateraccountingframework-530x412.jpg)
*Water Accounting plus (WA+) principle*

## Manual

**Input data:**

1. Precipitation
2. Actual evapotranspiration
3. Land use/cover
4. Change in storage (surface, groundwater)
5. Ground data for validation (P, ET, river discharge)

**Tools:**

GIS: ArcGIS, QGIS, Excel

## Exercise

The objective of this exercise is to calculate some useful performance indicators for the Blue Nile Basin, which is a transboundary basin located in the Northeast Africa and shared between Sudan and Ethiopia. Data and working sheets are attached in the following [link](https://th-koeln.sciebo.de/s/cXUt1EqZZykQKmh)

**Data:**

Resource base sheet

Evapotranspiration sheet

**Working sheet:**

Excel file contains the indicators that should be calculated

## Example

Many case studies are available in the following link

<http://www.wateraccounting.org/projects.html>

Cambodia, Vietnam, Helmand, Incomati, Mara, Mekong, Volta, Naivasha, Nile, Sril Lanka, Awash, Okavango, East Rapti.
