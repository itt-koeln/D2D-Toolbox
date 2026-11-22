---
layout: default
title: "Rainwater harvesting potential using Multi Criteria Decision Analysis (MCDA) in GIS"
parent: Data Processing
grand_parent: D2D Toolbox
nav_order: 13
permalink: /toolbox/data-processing/rainwater-harvesting-potential-using-multi-criteria-decision/
---

# Rainwater harvesting potential using Multi Criteria Decision Analysis (MCDA) in GIS

*Posted 2018-06-21*

**Prepared by: Zryab Babker                                                   ![]({{ site.baseurl }}/assets/uploads/2018_06_gis.jpg)**

---

**1. Background**

The identification of potential sites for rainwater harvesting is an important step towards maximizing water availability and land productivity especially in water-scarce countries in arid and semi-arid regions. Geographic Information System (GIS) is powerful tools, which is used for pre-processing and then map creation of factors, which directly influence the process of selecting RWH locations. These maps are to be further processed and integrated together to produce one map for MAR suitable locations after taking into consideration all constraints.

**Multi-Criteria Decision Analysis (MCDA)** techniques in GIS environment is important for water resources management and used to compline different layers of special data representing the criteria and specify how those layers are combined. A combination of two methods of MCDA technique namely **Weight Liner Combination (WLC)** and **Boolean technique** which is implemented in ArcGIS, can be used for this objective. They can be used as well to check the suitability of the place for groundwater recharge among others. However, based on the review of the available studies in this topic, the selection of suitable thematic layers, the proper assignment, and analysis of weights for those layers as well as adopting realistic suitability criteria is the key to the success of selecting suitable locations for RWH structures.

---

**2. Principle**
**The boolean technique** is initially introduced by Robinov (1989) and is used to obtain constraints’ map using the variables ‘true or false’. A value of 1 will be assigned to each location specifying whether it is fulfilling a certain condition and 0 if it is not. This method is used to eliminate some sites that are considered unsuitable for RWH. Meanwhile, weight linear combination method (WLC) involves classifying each factor map to classes and assigning a score to each class depending on its suitability to locate RWH site. A weight will be assigned to each factor layer, which represents its comparative importance, and then the score of each map at each location will be combined to obtain a final map whereby an overall suitability score will be identified based on the following equation[[1]](#_ftn1):
**![]({{ site.baseurl }}/assets/uploads/2018_06_equation.jpg)**

Where Sj is the final suitability score in each pixel, Xij is the suitability of the ith cell with respect to the jth layer, and Wi is a normalized weight as the summation of Wi equal to 1.

This means places that are unsuitable for one criterion can still get a high class if all other criteria are valued suitable.

Comparing this method with other classical methods like SCS-CN method, it gives an accurate and detailed map for potential locations for RWH according to their suitability.

--------------------------------------------
[[1]](#_ftnref1) Malczewski, J., 1999. GIS and Multicriteria Decision Analysis. John Wiley & Sons,Inc.. 392 pp.

---

**3. Manual**
**Input data:**

A mixed of physical and socioeconomic criteria (factors) is needed for selecting the suitable sites for the RWH.

- Example of physical criteria:

1. Slope map
2. Geology map of the area
3. Soil map
4. Drainage density
5. Land use/ land cover
6. Rainfall

- Example of socioeconomic criteria:

1. Distance to Roads
2. Distance to international borders
3. Urban areas

**Process:**

- First, each on of physical criteria should be imported in GIS, converted to raster, and reclassified according to certain classifications. Then using WLC method in raster calculator, all these maps will be integrated based on Equation 1 above to form primary map RWH suitability, which is classified into different classes from low to high suitability.

A buffer zone will be applied to all socioeconomic factors according to their economic or safe distance from the aforementioned criteria. Then union tool in GIS is to be used for spatially merging the buffer zones of each socioeconomic criterion with the selected study area to incorporate the areas beyond the selected zone distances. After that, the Boolean technique will be applied to create a constraint map by selecting all areas which are not suitable for RWH site selection

- Finally, the primary map should be masked with the constraints to produce the final RWH site suitability map

- The above-mentioned procedure is illustrated in the following graph:

![]({{ site.baseurl }}/assets/uploads/2018_06_mar.jpg)

---

**4. Exercise**

This procedure can be applied to any selected case study if the needed input data are available

---

**5. Example**

Many case studies are available in the literature which use these techniques to select suitable locations for either Rainwater Harvesting (RWH) or Managed Aquifer Recharge (MAR).

**Examples of literature:**

Abdel Rahman Al-shabeeb (2016) The use of AHP within GIS in selecting potential sites for water harvesting sites in Azraq Basin- Jordan. Journal of Geographic Information System, 8, 73-88. <http://dx.doi.org/10.4236/jgis.2016.81008>
Madan K. Jha, V.M. Chowdary, Y. Kulkarni, and B.C. Mal. (2014) Rainwater harvesting planning using geospatial techniques and multicriteria decision analysis. Resources, Conservation and Recycling; 83, 96-111
