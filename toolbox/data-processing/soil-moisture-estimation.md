---
layout: default
title: "Soil moisture estimation"
parent: Data Processing
grand_parent: D2D Toolbox
nav_order: 16
permalink: /toolbox/data-processing/soil-moisture-estimation/
---

# Soil moisture estimation

*Posted 2018-06-21*

**Prepared by: Elmoiz Yousif Elnayer Taha**

![]({{ site.baseurl }}/assets/uploads/2018_06_soilmositure.jpg)

---

**1. Background**

Among all the hydrologic variables, soil moisture is one of the least measured variables for understanding droughts at large spatial scales (Manohar et al., 2016), increased interest in soil moisture information for applications in such disciplines as hydrology, meteorology, and agriculture has necessitated an overview of both existing and proposed methods for determination of soil moisture([Schmugge](https://agupubs.onlinelibrary.wiley.com/action/doSearch?ContribAuthorStored=Schmugge%2C+T+J) et al., 1980). Soil moisture may be measured by a variety of methods, but unfortunately, there is no comprehensive, national network of soil moisture monitoring instruments (Keyantash and Dracup. 2002). Droughts are one of the costliest natural disasters and globally affect a large number of people and their livelihoods every year.

---

**2. Principle**

There are many good reasons for the study of soil and plant water relations. The amount of water in soil and plants plays a fundamental role in the control of land surface processes now proving so important to understanding local and regional climatology, Estimation of SM is considered very useful of many water- budgeting operations such as agricultural applications (Ahmad et al., 2017; Peng and Loew, 2017).  The water balance is an accounting of the inputs and outputs of water. The water balance of a place, whether it be an agricultural field, watershed, or continent, can be determined by calculating the input, output, and storage changes of water at the Earth's surface. The major input of water is from precipitation and output is evapotranspiration. The geographer (C. W. Thornthwaite 1899-1963) pioneered the water balance approach to water resource analysis. He and his team used the water-balance methodology to assess water needs for irrigation and other water-related issues.

![]({{ site.baseurl }}/assets/uploads/2018_06_soilmositure2-530x447.jpg)

![]({{ site.baseurl }}/assets/uploads/2018_06_soilmositure3-530x341.jpg)

Soil Water Deficit Index SWDI developed by (Martinez et al., 2015) It has shown good results to detect the agricultural drought based on soil moisture, as it deals directly with the Available Water Content (AWC), which in field of agricultural drought could be more important than soil moisture itself (Zamora et al., 2016) .This index is able to identify the attributes that define drought event, and given by the following equation:

![]({{ site.baseurl }}/assets/uploads/2018_06_soilmositure4.jpg)

Where θ is the soil water content. FC denotes field capacity and AWC is the available water content, which is the difference between FC and permanent wilting point (WP), when SWDI is above zero, the soil has a surplus of water; when it equals zero, the soils at the field capacity in terms of water content (i.e., no water deficit and no drought). While negative values indicate agricultural drought and its impacts will depend on the type of crop and the fraction of total available soil water that can be depleted from the root zone before moisture s occurs (Martinez et al., 2016).

---

**3. Manual**

**Input data:**

1. Precipitation
2. SMAP soil Moisture (Surface and Root-Zone)

**Tools:**

GIS: ArcGIS, QGIS, Excel

---

**4. Exercise**

- You can use this index in order to retrieve soil moisture as available water content/or not available for crops in different crop life cycles.
- No exercise available.

---

**5. Example**

Many case studies are available:

1. Martínez-Fernández, A. González-Zamora, N. Sánchez, A. Gumuzzio, and C.M. Herrero-Jiménez (2016). Satellite soil moisture for agricultural drought monitoring: Assessment of Remote Sensing of Environment, pp 277-286
2. Martínez-Fernández, A. González-Zamora, N. Sánchez, A. Gumuzzio, and C.M. Herrero-Jiménez, (2016). Satellite soil moisture for agricultural drought monitoring: Assessment of the SMOS derived Soil Water Deficit Index, Journal of Remote Sensing for Environment, pp 277-286.
3. Angel González-Zamora, Nilda Sánchez, José Martínez-Fernández, Wolfgang Wagner (2016). Root-zone plant available water estimation using the SMOS-derived soil water index, Advances in Water Resources, pp339–353.
