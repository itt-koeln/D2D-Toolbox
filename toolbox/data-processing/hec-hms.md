---
layout: default
title: "HEC-HMS"
parent: Data Processing
grand_parent: D2D Toolbox
nav_order: 6
permalink: /toolbox/data-processing/hec-hms/
---

# HEC-HMS

*Posted 2018-06-13* · Category: Rainfall-Runoff modelling

**Prepared by: Mohammed Basheer**

![]({{ site.baseurl }}/assets/uploads/2018_06_hechms.png)

---

### **1. Background**

The Hydrologic Engineering Centre - Hydrologic Modelling System (HEC-HMS), developed by the Hydrologic Engineering Centre (HEC), is a computer program that includes a broad set of mathematical models that simulate rainfall-runoff of dendritic watershed systems with a wide range of time steps (from one day to one minute). HEC-HMS is capable of calculating runoff volume, baseflow, soil infiltration, canopy interception, surface storage and evapotranspiration, and channel flow.  Moreover, the Hydrologic Engineering Centre - Geospatial Hydrologic Modelling System (HEC-GeoHMS), a geospatial hydrologic modeling extension developed by HEC, can be used to delineate sub-basins and streams, determine their geometric characteristics, and construct inputs to HEC-HMS.

It is essential to link HEC-HMS with rainfall products evaluation tools such as R, Python, and ArcGIS. Moreover, land cover classification tools could also be linked to HEC-HMS (e.g. R and ArcGIS).

**References:**

HEC (2000) Hydrologic Modeling System HEC-HMS Technical Reference Manual. Washington. Available at: [here](https://th-koeln.sciebo.de/s/wsjlog7YPsU98sY).

HEC (2009) *HEC-GeoHMS Geospatial Hydrologic Modeling Extension: User’s* *Manual*. Washington.

---

### **2. Principle**

HEC-HMS simulates the physical processes mentioned in section one using a variety of mathematical models which include event models, continuous models, lumped models, distributed models, empirical models, conceptual models, and deterministic models. Mass conservation is the basis of all mathematical models in HEC-HMS.

---

### **3. Manual**

HEC-HMS source file can be downloaded from HEC website (<https://www.hec.usace.army.mil>) and can be installed straightforward. HEC-HMS is open source. Therefore, no license is required to use it.

Typical data required to develop a HEC-HMS model include rainfall, topography, soil, land use/land cover, evapotranspiration, and some flow data to calibrate the model and to construct the baseflow. The amount of additional data required depends on the mathematical models selected to simulate the physical processes.

HEC-HMS is an object-based software which means that objects are to be added to the workspace, connected with each other, and populated with methods and data.

HEC-HMS can be run in several modes: simulation, optimization, forecast, depth-area analysis, and uncertainty analysis.

---

### **4. Exercise**

Attached find raw data required to develop a simple simulation model for Rio Tibag Basin (Brazil) using HEC-HMS. The attachment in the following [link](https://th-koeln.sciebo.de/s/wsjlog7YPsU98sY) includes rainfall and discharge data. Additionally, a report on the results of the same exercise model is also attached.

---

### **5. Example**

HEC-HMS has been used to conduct a study which can be accessed from the following link: <https://www.researchgate.net/publication/245289459_Event_and_continuous_modeling_with_HEC_HMS>
