---
layout: page
title: Tool 10 - Rooftop Rainwater Harvesting Calculator
permalink: /Rooftop_Rainwater_Harvesting_Calculator/
parent: TOOLKIT - Water-Sensitive Infrastructure Development
grand_parent: Projects
nav_order: 11
---

![Banner]({{ site.baseurl }}/assets/Headers/Rooftop Rainwater Harvesting Calculator.png){: style="width:100%; height:auto;" }



# Tool 10: Rooftop Rainwater Harvesting Calculator
_Authors: Samuel Edward Hume_

This tool allows for the calculation of the Rainwater Harvesting (RWH) potential of different rooftop catchments. This refers to how much water can be collected by a rooftop or groups of rooftops. The tool uses average monthly precipitation and the rooftop surface area and material. A tank size to store excess water is suggested if water demand data is available.

|        |  Rooftop Rainwater Harvesting Calculator      |
|:-------------|:------------------|
| **What?** | The tool calculates the amount of rainwater that can be harvested from rooftop catchments using the parameters for the rooftop catchment and precipitation data. It also estimates a tank size based on the scenario. Outputs: <br>• Monthly and Annual Rainwater Harvesting Potential<br>• Supply to Demand Surplus or Deficit<br>• Approximate Tank Size |
| **Why? / Purpose** | To evaluate whether implementing rooftop rainwater harvesting systems is beneficial in case studies.<br>The tool effectively calculates rainwater harvesting potential from rooftop catchments and can be used quickly and easily to quantify the potential supply and compare it to the demand.|
| **Field of Application** | The tool can be applied to any building or set of buildings. The scale can be from individual buildings to medium-sized urban districts. The context of tool use is urban areas with a need of a supplementary water supply or improved runoff storage.|
| **End Users** | •	Practitioners in the field of water engineers and urban planning. As well as governors from local and regional level<br>• Bachelor’s and master’s students of Engineering, Resource Management, Environmental Studies or related studies|
| **Background** | The idea developed through the interest in calculating how much water could be harvested from the rooftops considered in the water-sensitive park area in Sam Neua case study to support the Concept Note. It was decided to develop the tool concurrently so that these calculations could be easily done for other case studies. Tank sizing was then implemented so that there is a suggestion for the system as a whole.|
| **Description** | **Data Requirements**: Average Precipitation Data (Monthly or Annual), Water Demand (Monthly, per building), Rooftop Material, Rooftop Catchment Area<br> **Outputs:** <br>•	Monthly and Annual Rainwater Harvesting Potential: The amount of water that can be harvested each month, and total over the year.<br>•	Supply to Demand Surplus or Deficit: Takes the total RWH potential from the above calculation and the total yearly demand and calculates the difference<br>•	Approximate Tank Size: Calculates tank size based on volume of water would be used. Calculation depends on whether the RWH potential is greater or smaller than the total demand.|
| **Strengths and Limitations** | **Strengths:** Easy to use, simple data requirements, clear estimation of RWH potential, easy to compare different catchments and easy to switch between scenarios. <br> **Limitations:** Requires specific demand data to properly inform about the potential benefits of a RRWH system.  The tank sizing calculations don’t consider any economic aspects.|
| **Requirements  (Instruments Used)** | **Time:** Short, analysis for small groups of building can be done within a day<br> **Skills:** Basic knowledge of GIS and Excel. Moderate data processing skills for monthly precipitation data.<br> **Equipment:** Computers for spreadsheet access/data handling, images of the study area for rooftop characteristics, GIS to calculate areas.<br> **Costs:** Low. Potential site visits, data collection.|
| **Keywords** | Rainwater Harvesting, Rainwater Harvesting Potential, Runoff Coefficient, Hydrological Year |

## Tool Manual

### _a. Tool Oveview_

The tool allows the user to be able to calculate rainwater harvesting (RWH) potential for a given rooftop catchment based on the average monthly precipitation and rooftop material. The tool also suggests a tank size based on demand. 
The main application is to calculate the rainwater harvesting potential (VR).  This refers to the volume of water that can be collected from the rooftop over a period of time. The equation for this is as follows (Adugna et al., 2018; Hari et al., 2018; Villar-Navascués et al., 2020):
<p style="text-align: center;"><em>V<sub>R</sub>=A*P*C<sub>r</sub>.</em></p>

Where: V<sub>R</sub>=Rainwater harvesting Potential (m<sup>3</sup>); A = Catchment area (m<sup>2</sup>); P=Precipitation (m); C<sub>r</sub> = Runoff coefficient

The catchment area (A) refers to the rooftop area that will be used in the calculation. Depending on the scale and purpose of the use case, this area can reflect individual buildings or groups of buildings. The runoff coefficient (Cr) is the proportion of precipitation that becomes surface runoff. In other words, it is the fraction of rainfall that will be able to be stored. Each rooftop will have a slightly different Cr. It depends on the material and slope.
The tool also provides estimates for tank size based on the RWH potential and demand. The calculation depends on whether the RWH potential is greater or less than the demand. If the RWH potential is greater, then the tank size is one month’s demand plus the cumulative volume of the difference between RWH potential and demand in the months where demand is greater than RWH supply.


### _b. Tool Usage Steps_

### 1. Data Inputs

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/RRWH/Figure_52.png" alt="Figure_52" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 52: Data input steps for RRWH tool.</figcaption>
</figure>

1. <u>Add Precipitation Data:</u><br>
Add precipitation data in average monthly format. It is recommended to use the Climate Engine app (https://app.climateengine.org/climateEngine, Huntington et al., 2017) to download data from CHIRPS (C. Funk et al., 2015) if rainfall gauge data is unavailable. The data source can be indicated in the box. The month in which the hydrological year starts can be selected from a drop-down menu.  
2.	<u>Add Rooftop Catchment Data:</u><br>
The rooftop catchment data is formed of 4 components. First is the identifier of the catchment or catchment name. This should be easily identifiable and different from the other catchments being used in the analysis. The number of buildings within the catchment is then required. This allows for diverse applications of the tool and individual buildings or groups of different sizes. 
The rooftop material is taken from a table on the “Rooftop Material Types” sheet within the tool. Certain materials are already listed, however roof materials not included must be added to this table. The table requires the runoff coefficient of the material. This can usually be found in journal articles for common rooftop material types. Once a material is added on the “Rooftop Material Types” sheet, it will appear within the “Rooftop Material” column in the “Data Inputs” section. 
The Area refers to the total area of the catchment. Therefore, if multiple rooftops are being considered, this area should reflect the combined areas of all rooftops within the catchment. The area of rooftops can be determined using satellite imagery and GIS by drawing polygons. Additionally, Google Research provides a dataset “Open Buildings” that identifies buildings in the Global South: https://developers.google.com/earth-engine/datasets/catalog/GOOGLE_Research_open-buildings_v3_polygons#citation (Sirko et al., 2021). 
3.	<u>Add Demand Data:</u><br>
Demand data reflects how much water will be used. It is optional, as it difficult to quantify due to the water from RRWH being only suitable for certain uses but should be added if available. The quantity for different uses can be estimated in some cases. When available, the data allows for the visualisation of the relationship between the water able to be supplied from the system and the demand. Also, whether the supply can meet the demand. It also helps to refine the tank sizing process and discussed in Section 1.
4.	<u>Add Assumed Losses:</u><br>
Assumed losses account for inefficiencies within the system, losses from evaporation and small rainfall events that produce no runoff. The default value is 20%, however it can be refined if extra information is available. 


### 2. Select Outputs

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/RRWH/Figure_53.png" alt="Figure_53" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 53: Output selection box from RRWH tool.</figcaption>
</figure>

The selection interface (Figure 53) allows to select a rooftop catchment and demand from the data input tables. As multiple catchments and demands can be stored in the data inputs, switching between different combinations is simple and allows for comparisons to be made more easily.

### 3. Visualising and Interpreting Results

Results are found on the “Outputs” sheet. It is composed of tables and graphs. The table (Figure 54) displays the monthly RWH potential, cumulative monthly RWH potential and cumulative monthly demand. Additionally, the Annual total is displayed along with the annual volume collected per square meter. This value allows for easy estimations of rooftops with similar characteristics that weren’t considered in the analysis. 

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/RRWH/Figure_54.png" alt="Figure_54" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 54: Results Table, RRWH Tool.</figcaption>
</figure>

The annual surplus/deficit is displayed and is coloured coded depending on if it is negative or positive. It reflects whether the supply can meet the demand. A tank size is recommended based on the calculations described in Section 1, the suggested tank size rounds the calculated size to a regular tank size.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/RRWH/Figure_55.png" alt="Figure_55" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 55: Cumulative RWH Potential and Demand monthly time series, RRWH Tool.</figcaption>
</figure>

The graph allows for a visualisation of the trend between RWH potential and demand. It is useful for seeing deficits in dry season or the reverse in wet season. The final endpoint of each line shows whether the potential exceeds the demand over the course of the year or not.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/RRWH/Figure_56.png" alt="Figure_56" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 56: Results Table, RRWH Tool.</figcaption>
</figure>

Figure 56 is an output graph that shows the RWH potential of different rooftop areas. The range of sizes is determined from the areas already entered into the “Rooftop Catchment Characteristics”.

## Study Case

The tool was used to assess the potential of Rooftop Rainwater Harvesting (RRWH) in Sam Neua, Laos, as part of the town's Multi-functional Park development. The area comprises of 15 residential and 3 public buildings as pilot sites.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/RRWH/Figure_57.jpg" alt="Figure_57" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 57: Map of the Park area and buildings selected for RRWH implementation.</figcaption>
</figure>

The area has a temperate dry winter-hot summer climate (Cwa) (Kottek et al., 2006). This gives the region distinct dry and wet seasons and an annual average precipitation of 1324.87mm.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/RRWH/Figure_58.png" alt="Figure_58" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 58: Average Monthly Precipitation in Sam Neua Park, Laos. Source: Funk et al.( 2014)</figcaption>
</figure>

The total rainwater that could be harvested for the buildings is large, with nearly one cubic meter of water being collected per 1m<sup>2</sup> of rooftop. In the case of Sam Neua, RRWH shows great promise. For the public buildings, it shows that over the course of the year, 1745.59m<sup>3</sup> of water could be harvested overall to supplement water supply. The amount of water that can be supplied is lower than the demand of the buildings. Therefore, tank sizing is determined by calculating the amount of excess water that can be harvested over the wet season whilst considering monthly abstractions to meet demand. For the public buildings, the potential supply also doesn’t meet to the total demand. There is an overall deficit of -262.7m<sup>3</sup> yearly. The suggested tank size is 200m<sup>3</sup> from a calculated potential storage volume of 192.87m<sup>3</sup> per building. There is a large amount of water that can be potentially supplied. The tank sizing is a concern as the calculated volume is very large. Private buildings can theoretically collect 1913.66m<sup>3</sup> of water per year overall. With 15 buildings, the individual calculated storage volume considering constant water abstraction for each household would be 35.37m<sup>3</sup> meaning a suggested tank size of 40m<sup>2</sup>. This would provide a significant amount of water for each household. However, it is likely the costs of providing these tanks would also be too great.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/RRWH/Figure_59.png" alt="Figure_59" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 59: Results output page for Private buildings.</figcaption>
</figure>

The results show that over the course of the year that the RWH potential was less than the total demand (Figure 59). However, the demand used was an estimation of total household demand. The amount of water supplied would likely cover the uses that harvested rainwater is suitable for. Due to the pronounced seasonality, the suggested tank size is large.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/RRWH/Figure_60.png" alt="Figure_60" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 60: RRWH potential and demand curves plotted cumulatively for different roof sizes, using CPAC concrete tiling as the roof material.</figcaption>
</figure>

The rooftop size necessary to meet the demand for both private and public buildings are realistic sizes met by multiple buildings within the study area. It is shown that to meet the average household demand, a roof size of approximately 180m<sup>3</sup> is needed (Figure 60). A few of the households meet this requirement. For the Government office demand, a roof size of 700m<sup>3</sup> would be needed.

## Access to the tool

The tool can be accessed <a href="https://th-koeln.sciebo.de/s/7OsT6OvK8MXWC1x" target="_blank" rel="noopener noreferrer">**here**</a>, along with the supporting documentation.

## Further Reading

Abdulla, F. (2020). Rainwater harvesting in Jordan: potential water saving, optimal tank sizing and economic analysis. Urban Water Journal, 17(5), 446–456. https://doi.org/10.1080/1573062X.2019.1648530

Siddiqui, R., & Siddiqui, S. (2018). Assessing the Rooftop Rainwater Harvesting Potential in Urban Residential Areas of Pakistan: A Case Study of Model Town, Lahore, Pakistan. Int.J.Econ.Environ.Geol, 9(2), 11–19. https://www.researchgate.net/publication/343139795

Villar-Navascués, R., Pérez-Morales, A., & Gil-Guirado, S. (2020). Assessment of rainwater harvesting potential from roof catchments through clustering analysis. Water (Switzerland), 12(9). https://doi.org/10.3390/W12092623

Adugna, D., Jensen, M. B., Lemma, B., & Gebrie, G. S. (2018). Assessing the potential for rooftop rainwater harvesting from large public institutions. International Journal of Environmental Research and Public Health, 15(2). https://doi.org/10.3390/ijerph15020336

