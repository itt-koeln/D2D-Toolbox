---
layout: page
title: Tool 11 - Hydrological and Hydraulic Modelling 
permalink: /Hydrological_and_Hydraulic_Modelling/
parent: TOOLKIT - Water-Sensitive Infrastructure Development
nav_order: 12
nav_exclude: true
---

![Banner]({{ site.baseurl }}/assets/Headers/Hydrological and hydraulically modelling.png){: style="width:100%; height:auto;" }


# Tool 11: Hydrological and Hydraulic Modelling 
_Authors: Samuel Edward Hume, Lina Rocio Pérez Corredor, Juan Miguel Viquez, Frederic Hebbeker, Yagana Yusufi_

Hydrological and Hydraulic modelling tool provide many opportunities to investigate problems and solutions to water management issues. This tool applies methodologies to existing modelling software to produce results that can be used in designing and improving water sensitive urban design in secondary and tertiary cities in SEA. The first methodology uses HEC-RAS to provide a hydrodynamic model of an urban area using a detailed elevation model from drone imagery (see Drone Survey) combined with infiltration maps and precipitation data. The main output is a runoff map that helps to identify areas of accumulation during storm events, highlighting areas that would benefit most from NbS implementation. The second methodology uses SWMM to assess rainfall-runoff dynamics and evaluate the performance of urban drainage systems under various design storm events with different return periods. The analysis aims to identify flood-prone areas by assessing the capacity of the drainage infrastructure, pinpointing potential inundation zones, and determining the extent and severity of flooding using LULC, soil and elevation data. The method highlights critical areas that require improvements or redesign to enhance flood mitigation. 

|        |  Hydrological and Hydraulic Modelling       |
|:-------------|:------------------|
| **What?** | The tool comprises two widely-used, open-access software applications—SWMM (Stormwater Management Model) and HEC-RAS (River Analysis System)—designed for hydrological and hydraulic modelling in urban and river basin environments.  These tools simulate pluvial flooding on an urban scale, essential for understanding flood risks and runoff management.<br> **Main Characteristics:**<br>•	HEC-RAS: Conducts 1D and 2D hydraulic modelling of river systems, enabling the simulation of river hydraulics, surface flow dynamics, and runoff impacts.<br>•	SWMM: Models the rainfall-runoff process in urban environments, simulating stormwater management and assessing how urban drainage systems respond to precipitation events, including both runoff and water quality.|
| **Why? / Purpose** | The purpose of this tool is to support decision-making for water-sensitive urban planning by providing precise simulations of water flows. It helps identify flood-prone areas, evaluate the effectiveness of Nature-based Solutions (NbS), and design sustainable infrastructure systems.  |
| **Field of Application** |  The methodologies are best suited to a municipality-level scale, small-medium sized urban areas. Larger areas are possible but have greater computational requirements.|
| **End Users** | Urban planners and municipal water managers. Environmental and hydrological consultants, policymakers and local governments in secondary and tertiary cities, academics and researchers. |
| **Background** | These tools are globally adapted for hydrological challenges. These tools have been adapted in the (PUW) project for Southeast Asian (SEA) cities, incorporating regional hydrological data, localized flooding challenges, and participatory planning approaches. |
| **Description** | **HEC-RAS**: A detailed surface elevation model is used as the base terrain for the model. Within the model, infiltration data derived from soil type and land-use cover is overlayed onto the terrain. Design storm events are then integrated into the model which then provides the surface runoff and flow direction, allowing for the visualisation of runoff accumulations and potential flood risk zones.<br> **SWMM**: Simulates urban runoff using sub catchment data, drainage networks, and rainfall inputs, incorporating NbS interventions and evaluating system performance under storm events.|
| **Strengths and Limitations** | **Strengths:** Integrates hydrological and hydraulic modelling for detailed, scenario-based assessments. Helps develop an understanding of the hydrology of the area. Visualizes outputs to effectively communicate results to stakeholders. Versatile application across urban and river basin contexts. <br> **Limitations:** Relies on accurate and high-resolution DSM/DTM data, difficult to calibrate, requires experience with the respective software. Requires extensive input data (e.g., precipitation, elevation) which may not always be available. High technical expertise needed for model setup, calibration, and interpretation. Computationally intensive for large-scale applications.|
| **Requirements  (Instruments Used)** | **Time:** Moderate to long (for data preparation, calibration, and scenario analysis).  <br> **Skills:** Hydrological and hydraulic modelling expertise, GIS knowledge.<br> **Equipment:** HEC-HMS, HEC-RAS, SWMM, GIS tools.  <br> **Costs:** Moderate (primarily for training and data acquisition). |
| **Keywords** | Hydrological Modelling, Hydraulic Modelling, Land Use – Land Cover, Surface Runoff, Pluvial Flooding, Fluvial Flooding. |

## Tool Manual

### _a. Tool Oveview_

Hydrological and hydraulic modelling is a valuable tool in urban water management. It can serve multiple applications, including determining flood extent, designing dams and analysing drain networks. Within the project, models were identified as a useful tool to gain insights into the hydrology of the pilot areas. Specifically, the models were designed to determine the runoff from urban areas and identify where it accumulates. This allows for the identification of risk zones for urban flooding and also helps highlight areas that would benefit most from the implementation of NbS. Drone data was collected to for the base of the models, and these were used in combination with open-source datasets to produce the models.


**Objectives:**
-	Identify areas prone to high surface runoff and runoff accumulation
-	Identify flood-prone areas, evaluate drainage capacity, highlight critical areas for improvement.


### _b. Tool Usage Steps - HEC-RAS_

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 61.png" alt="Figure_61" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 61: Flow chart of HEC-RAS methodology. Source: ITT 2024.</figcaption>
</figure>


### 1. Prepare Data

1.	**Precipitation Data:** Use a long-term historical precipitation dataset. If rain gauge data or higher temporal resolution data is unavailable, the MSWEP V2.8 3-hourly historical precipitation dataset is recommended. Extraction of timeseries of this data can be accomplished using the Insight for Urban Water Management Using Open-Source Data tool.  If rain gauge data or similar is available, it is preferred over MSWEP data.
2.	**Terrain Model:** A digital terrain model (DTM) is used. It can be derived through photogrammetry with adapted SMRF (simple morphological filter) parameters (see Drone Survey tool). In order to best represent the surfaces that impact runoff, houses should be included from the DSM, based on open building data, corrected with a high resolution orthomosaic. The DTM is resampled to a resolution of 0.5 meters, balancing computational efficiency and terrain representation accuracy. It is added as a Terrain layer in RAS Mapper as a .tif file. 
3.	**Study Area:** Add a shapefile of the study area as a polygon in RAS Mapper. 
4.	**Land Use and Land Cover (LULC):** Collect Land Use/Land Cover (LULC) data and Hydrological Soil Group (HSG) data for the study area. Global LULC datasets, such as the GLC Share Database (FAO) or Worldcover (ESA), are usually sufficient for the model. Photogrammetry from drones can be used to improve classifications (see Drone Survey tool); Each LULC classification also needs a Mannings coefficient. The SWMM User’s Manual Version 5.2 Table A.6 (Rossman & Simon, 2022) can be used for approximating this value. 
5.	**Soil Data:** Obtain soil data to determine the HSG of the study area. A global dataset for HSG is available at the ORNL DAAC website (Ross et al., 2018).
 


### 2. Data Processing - GIS

1.	Process spatial datasets, including precipitation, terrain, LULC, and soil data, using ArcGIS or equivalent GIS software.
2.	Ensure layers are pre-processed to align spatially and are in the same coordinate reference system.


### 3. Design Rainfall Events

Use the **Frequency Storm Method** in HEC-HMS, relying on Depth-Duration-Frequency (DDF) data. The DDF durations are 3, 6, 9, 12, 24, and 48 hours, and return periods: 1, 2, 5, 10, 30, 50, and 100 years. Perform a DDF analysis using a long-term historical precipitation dataset. Use a Python package developed by (Pichler, 2024)  for DDF analysis. Generate a DDF table for the study area. Input precipitation values from the DDF table for each duration and return period. Generate a precipitation time series for the storm event using the Frequency Storm Meteorological Method in HEC-HMS.

### 4. HEC-RAS Development
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 62.png" alt="Figure_62" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 62: Stages of the construction of the HEC-RAS model</figcaption>
</figure>

1.	**Study Area:** Add the study area shapefile as a reference layer in RAS Mapper.
2.	**Terrain Model:** Import the DSM into RAS Mapper as a terrain layer.
3.	**2D Flow Area:** Add a 2D Flow Area under "Geometries" in RAS Mapper. Draw the perimeter of the flow area around the study area but within the terrain's limits. Add computational points spaced according to the terrain resolution and calculate the computational grid.
4.	**Infiltration layer:** Combine LULC data with HSG using RAS Mapper to create a new intersected polygon layer. Refer to Curve Number (CN) tables in the HEC-HMS Technical Reference Manual (USACE, 2024.) to assign CN values to the polygons. Initial Abstraction is assumed to be 0.1. Minimum infiltration rate is determined by the soil type, according to the HEC-RAS Technical Reference Manual.
5.	**Boundary Conditions:** Add boundary conditions under "Geometries":<br>
o Perimeter Boundary Condition: Define the perimeter of the 2D Flow Area.<br>
o	Normal Depth Boundary Condition: Set for water outflow at the model boundaries.<br>
Input the appropriate hyetograph for the precipitation event at the 2D flow area boundary.
6.	**View/edit Unsteady Flow Data:** The 2D flow area requires 2 boundary conditions. The boundary condition line uses normal depth to allow flow out of the 2D flow area. The second boundary condition is for the 2d flow area perimeter, which is how the precipitation event is defined. Here, the matching hyetograph from the chosen storm event is entered.
7.	**Unsteady Flow Analysis:** The programs set to run are the Geometry Preprocessor, Unsteady Flow Simulation, Post Processor and Floodplain Mapping. The computation settings used are a computation interval of 5 minutes, with the hydrograph output, mapping output interval and detailed output interval are all set to 10 minutes.  
8.	**View Results:** The results can be views in RAS Mapper. **The key output is the water depth throughout the event**. This can be used to identify areas which see a high accumulation of runoff or high flow. Profile lines can be added to these areas of interest, which allows for the plotting of cross sections that show the water depth over the terrain using Water Surface Elevation (WSE) data. 


### _c. Tool Usage Steps - SWMM_

### 1. Required Data and Processing

1. **Precipitation**
   High-resolution precipitation data, preferably minute- or hourly-scale, are required for accurate modelling. Short intervals are ideal for small areas, while hourly data suffices for larger regions (Rossman, 2015). In the absence of local data, reanalysis datasets like MSWEP V2.8 (3-hour resolution) offer a viable alternative, combining satellite, ground, and model data for reliable simulations.

2. **Design Rainfall Events**
   Use the Frequency Storm Method in HEC-HMS, relying on Depth-Duration-Frequency (DDF) data. The DDF durations are 3, 6, 9, 12, 24, and 48 hours, and return periods: 1, 2, 5, 10, 30, 50, and 100 years. Perform a DDF analysis using a long-term historical precipitation dataset. Use a Python package developed by Pichler, M. (2024) for DDF analysis. Generate a DDF table for the study area. Input precipitation values from the DDF table for each duration and return period. Generate a precipitation time series for the storm event using the Frequency Storm Meteorological Method in HEC-HMS.

3. **Catchment Parameters Data**
   - **Topographic Data:**
     The digital terrain model with the resolution of (0.5m) derived from Drone (Hebbeker, 2025) is used for delineating catchment boundaries and identifying drainage patterns and primarily used ArcGIS Pro for the delineation.
   - **Land Cover and Soil Data:**
     Collect Land Use/Land Cover (LULC) data and Hydrological Soil Group (HSG) data for the study area. Global LULC datasets, such as the GLC Share Database (FAO) or Worldcover (ESA), are usually sufficient for basin-scale models. Obtain soil data to determine the HSG of the study area. A global dataset for HSG is available at the ORNL DAAC website (Ross et al., 2018).
   - **Infiltration Method:**
     The Curve Number (CN) method is applied to model soil infiltration in sub catchment areas. This empirical method, based on the SCS Curve Number derived from the SWMM user manual (Rossman, 2015) table A4, based on land use and hydrologic soil groups, with adjustments for mixed land uses.
   - **Catchment Parameters:**
     The subcatchment area are calculated using ArcGIS Pro. Slope are determined by importing a Digital Terrain Model (DTM) into ArcGIS Pro, generating slope rasters, and calculating average slopes using the Zonal Statistics tool. Subcatchments widths are estimated using the Skew Factor formula, which adjusts the channel length based on the ratio of larger to total areas on either side of the drainage channel, ensuring accurate representation of irregular shapes (Rossman, 2016). Imperviousness is calculated using land cover, soil, CN maps and predefined percentages from SCS TR-55 guidelines. Depression storage and Manning’s n values were calculated as weighted averages based on land cover types, using SWMM guidelines (Rossman, 2015).

4. **Drainage System Data**
   - **Junctions and Conduits:**
     A single vector layer combining drainage and river networks was used to model conduits, with junctions and outfalls represented in separate layers for their distinct purposes. A Manning’s n value, in line with SWMM recommendations, was applied to the conduits, ensuring consistency with standard flow modelling practices (Rossman, 2015).
   - **Junction and Conduit Configuration:**
     Conduits are defined by their inlet and outlet junctions to ensure proper flow direction, with flow moving from higher to lower elevations. Junctions were configured with invert elevations and maximum depths for correct flow modeling (Rossman, 2015). Conduit dimensions can be adapted based on studies from similar regions, when site-specific data is not available. Junction invert elevations are derived by extracting surface elevations from a Digital Terrain Model (DTM) using GIS tools, then subtracting the channel depth to accurately represent flow behaviour.


<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 63.jpg" alt="Figure_63" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 63. Sub catchments division and representation of drainage system in Rejodani sub-villages I and II, Indonesia. Source: ITT 2024</figcaption>
</figure>

### 2. Model Construction and Setup
Spatial features like sub-catchments, outfalls, junctions, and conduits are prepared as GIS shapefiles and then converted into the SWMM INP format for simulation. This is done using the "Generate SWMM INP" plugin in QGIS. The shapefile’s attribute table must include required fields for the conversion to work, while optional fields can be left empty if not needed. After confirming the attribute tables are filled, the plugin creates the INP file, integrating the data into the SWMM simulation.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 64.png" alt="Figure_64" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 64. QGIS format conversion to SWMM input. Source: ITT 2024</figcaption>
</figure>

In the model construction phase, several key steps are applied to run the models effectively. First, the rain gauge is set for each storm event duration (48H, 24H, 12H, 6H, and 3H) and their associated return periods (1Y, 2Y, 5Y, 10Y, 30Y, and 50Y). The parameters for sub-catchments, junctions, outfalls, and conduits, as outlined earlier, are carefully reviewed to minimize any errors in the model.
The SWMM simulation options are configured based on the storm's characteristics and the system's response to rainfall. By setting up these configurations, the model is run for each return period and duration.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 65.jpg" alt="Figure_65" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 65: SWMM sub-catchments division and representation of drainage system. Source: ITT 2024</figcaption>
</figure>


## Study Case

### a. HEC-RAS Method: Rejodani I + II

The HEC-RAS method was applied to the sub-villages Rejodani I + II in the pilot city of Sleman, Indonesia. The objective was to identify areas that may have a risk of flooding under extreme precipitation events.
Precipitation data was taken from MSWEP V2.8, which is a 3-hourly global precipitation reanalysis data product for the period 1979-2020 (Beck et al., 2019). Depth-duration-frequency (DDF) curves were derived using Python, with a package created by Pichler, M. (2024). HEC-HMS was used to apply the Frequency Storm method to derive storm event hyetographs (see Fig. 66).  


<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 66.png" alt="Figure_66" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 66. Storm event hyetograph for a storm duration of 12 hours and return period of 50 years. Source: ITT 2024</figcaption>
</figure>

A drone survey, conducted in October 2023 was used to derive DSM & DTM, adapting SMRF- parameters to increase the quality of Digital Terrain models, recommendable, especially in urban area (see Pingel et al., 2013). To enable not only the terrain runoff, but also runoff from houses, buildings footprints, based on Sirko et al., (2021), were adapted with the derived high resolution orthomosaic and used to clip them from the DSM and insert them into the DTM.
The LULC used was from the ESA Worldcover 2021 dataset (Zanaga et al., 2022) with some reclassifications performed using imagery from the drone survey to improve accuracy. This was intersected with hydrological soil group data from Ross et al. (2018) using RAS Mapper. These were used to derive a CN map of the area. The CN of the study area ranges from 79 in forest areas to 95 in densely built-up areas. The high CN reflects the urbanised nature of the catchment and also the clayey soil type. 


<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 67.png" alt="Figure_67" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 67. Instantaneous flood depth map and maximum flood depth cross sections at selected Areas of Interest for a 12hr storm event with a 50-year return period. Water Surface Elevation shown for: a) “Outflow west side” b) “Main Street” c) “Commercial Centre” d) “Housing Estate”. Source: ITT 2024</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 68.png" alt="Figure_68" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 68. Instantaneous flood depth map and maximum flood depth cross sections at selected Areas of Interest for a 12hr storm event with a 10-year return period. Water Surface Elevation shown for: a) “Outflow west side” b) “Main Street” c) “Commercial Centre” d) “Housing Estate”. Source: ITT 2024</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 69.png" alt="Figure_69" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 69. Instantaneous flood depth map and maximum flood depth cross sections at selected Areas of Interest for a 12hr storm event with a 5-year return period. Water Surface Elevation shown for: a) “Outflow west side” b) “Main Street” c) “Commercial Centre” d) “Housing Estate”. Source: ITT 2024</figcaption>
</figure>

The results of the model highlighted several areas which have high water depths throughout the event. Of these, 4 were selected as Areas of Interest (AOI). For these areas, cross section showing the elevation and water surface elevation were taken for the highest flood depth at each point. Flood depths in most of the AOIs showed flood depths of over 1m in the events, which is a depth which could cause damage to buildings and infrastructure. Overall, the flood depths associated with more extreme flood events only showed minor increases in flood depth at the AOIs. The RP50 event had a max flood depth of around 20cm higher than the RP5 event. However, larger areas of the study area had water depths of over 0.5m during the RP50 event. A notable trend was that the AOIs typically saw multiple flood waves as runoff travelled down the catchment from different parts of the study area. 

Additionally, photos of the AOIs were taken with the modelled flood depths for the different return periods marked (Fig. 70-71).

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 70.jpg" alt="Figure_70" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 70. Photo of “Main Street” area, a selected area of interest, with overlayed simulated flood levels for a 12hr storm for each event for return periods of 5-year to 50-year. Source: ITT 2024.</figcaption>
</figure>
<br>
<br>
<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 71.jpg" alt="Figure_71" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 71. Photo of “Commercial Centre” area, a selected area of interest, with overlayed simulated flood levels for a 12hr storm for each event for return periods of 5-year to 50-year. Source: ITT 2024</figcaption>
</figure>

### b. SWMM: Rejodani I + II
The rainfall-runoff simulation results across various return periods (100 years to 1 year) and a 12-hour duration have highlighted significant vulnerabilities in the drainage system (Fig. 72). The higher return periods, such as 100 years, 50 years, and 30 years, pose significant flood risks, with certain junctions consistently reaching their full capacity during extreme events.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 72.jpg" alt="Figure_72" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 72. Representation of Sub catchments and Drainage System. Source: ITT 2024</figcaption>
</figure>

For example, in the 100-year return period, junctions such as J12, J14, J15, J20, and J18 are particularly vulnerable, as they consistently reach full capacity, indicating a high risk of flooding during severe storms. Similarly, in the 50-year return period, junctions J12, J18, J14, and J20 are under significant stress, reaching full capacity and showing a clear potential for localized flooding. In the 30-year return period, J12, J18, and J20 remain at full capacity, signalling ongoing flood risks in these areas (Fig. 73). Junctions J6, J13, J21, J11, and O5 also show depths approaching critical levels, requiring attention (Fig. 74). 

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 73.png" alt="Figure_73" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 73. Reported Maximum Depth (m) of Junctions and Outfalls for Duration 12 Hours. Source: ITT 2024</figcaption>
</figure>

Similarly, conduits C12 and C25 demonstrate full depth ratios of 1.0 during extreme events of 100-year, indicating they are at full capacity, risking surcharging, while other several conduits such as C6, C11, C30, C38, C19, C22, C5, C18, and C23 approach critical levels (Fig. 74). These findings highlight key junctions and conduits under significant stress, requiring targeted mitigation measures to enhance system resilience.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 74.png" alt="Figure_74" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 74. Maximum Full Depth (m) of conduits for Duration 12 Hours. Source: ITT 2024</figcaption>
</figure>

As return periods decrease (10 years, 5 years, 2 years, 1 year), flood risk becomes more localized, with fewer junctions impacted and lower depths across the system. For example, in the 10-year event, flooding is limited to J12 and J18, and conduit performance improves, with reduced full depth ratios. Subcatchment S3 exhibit the highest runoff and peak flows, representing critical flood risks, while S1’s low infiltration exacerbates surface flooding potential. Conversely, S5’s low runoff and high infiltration effectively mitigate risk. Overall, the results emphasize prioritizing flood mitigation at critical junctions, conduits, and subcatchments identified under higher return periods, ensuring adequate capacity to manage stormwater during extreme events.

## Access to the tool

The tool can be accessed <a href="https://th-koeln.sciebo.de/s/TZgNdhBmV4AQLvX" target="_blank" rel="noopener noreferrer">**here**</a>, along with the supporting documentation.

## Further Reading

Pichler, M. (2024). idf_analysis: Intensity duration frequency analysis with python based on KOSTRA (v0.2.4). Zenodo. https://doi.org/10.5281/zenodo.10559992

Natarajan, S., & Radhakrishnan, N. (2020). An Integrated Hydrologic and Hydraulic Flood Modeling Study for a Medium-Sized Ungauged Urban Catchment Area: A Case Study of Tiruchirappalli City Using HEC-HMS and HEC-RAS. In Journal of The Institution of Engineers (India): Series A (Vol. 101, Issue 2, pp. 381–398). Springer. https://doi.org/10.1007/s40030-019-00427-2

Khatooni, K., Hooshyaripor, F., MalekMohammadi, B., & Noori, R. (2025). A new approach for urban flood risk assessment using coupled SWMM–HEC-RAS-2D model. Journal of Environmental Management, 374. https://doi.org/10.1016/j.jenvman.2024.123849

Rossman, L. A., & Huber, W. C. (2016). Storm Water Management Model Reference Manual: Volume I – Hydrology (Revised) (EPA/600/R-15/162A). U.S. Environmental Protection Agency, Office of Research and Development.

Rossman, L. A. (2017). Storm Water Management Model Reference Manual: Volume II – Hydraulics (EPA/600/R-17/111). U.S. Environmental Protection Agency, Office of Research and Development.
