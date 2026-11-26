---
layout: page
title: Tool 5 - Insights for Urban Water Management using Open-Source Datasets
permalink: /Insights_for_Urban_Water_Management_using_Open_Source_Datasets/
parent: TOOLKIT - Water-Sensitive Infrastructure Development
grand_parent: Projects
nav_order: 6
---

![Banner]({{ site.baseurl }}/assets/Headers/Identification and Assessments of Ecosystems Services (ES).png){: style="width:100%; height:auto;" }


# Tool 5: Insights for Urban Water Management using Open-Source Datasets
_Authors: Chahinaz Ziani_

Insights for Urban Water Management using Open-Source Datasets is a comprehensive assessment tool designed for urban and peri-urban watersheds. It provides step-by-step guidelines and R-scripts to analyze hydro-climatic parameters, evaluate hazards like droughts and floods, and assess trends in extreme weather events. The tool utilises open-source data to empower local authorities with data-driven decision-making capabilities, identify vulnerabilities, and implement proactive measures. 

|        |  Insights for Urban Water Management using Open-Source Datasets      |
|:-------------|:------------------|
| **What?** | This tool provides a step-by-step guideline for conducting a comprehensive assessment of watershed/urban hydrological processes. It offers an overview of the **hydroclimatic parameters** such as precipitation, evapotranspiration and temperature within the watershed that encompasses the urban study area, followed by an **evaluation of hydro-climatic hazards** such as **droughts and floods**, as well as **trends in extreme weather occurrences**. |
| **Why? / Purpose** | **Permitting data-driven decision-making**: Empowering local authorities to make informed decisions based on open data (without significant costs) <br> **Identification of vulnerabilities and implementing proactive measures**: by assessing hydroclimatic hazards (droughts, floods, extreme precipitation) <br> **Providing a comprehensive assessment of water management practices**: in the context of increasing urbanization and climatic variability, and as the study areas are transiting from rural to urban.|
| **Field of Application** | The tool can be applied at multiple scales, primarily focusing on urban and peri-urban areas within broader watershed contexts. The application of the can help for the formulation of a detailed water-sensitive development plan for secondary and tertiary cities. |
| **End Users** | •	Urban planners<br>•	Environmental scientists<br>• Community organizations (NGOs)<br>• Educational Institutions|
| **Background** | The tool was adapted to emphasize:<br>•	**Reanalysis Data Utilization**: Ensuring accessibility for municipalities with limited resources.<br>•	**Stakeholder Engagement**: Incorporating visual tools and guidelines that facilitate communication among various stakeholders involved in urban water management.<br>•	**Regional Relevance**: Tailoring methodologies to reflect local hydrological conditions and socio-economic contexts within Southeast Asia |
| **Description** | The tool is designed to facilitate a comprehensive assessment of watershed hydrological processes, specifically tailored for urban contexts.<br> •	It provides a structured framework and ready-to-use R-scripts for users to conduct a hydrometeorological baseline assessment<br>•	It enables the assessment various drought types—meteorological, hydrological, and agricultural<br>•	It incorporates a flood frequency analysis to evaluate flood risks. <br>•	It calculates precipitation extreme indices and analyses trends in extreme weather occurrences, all utilizing open-source data.<br> This integrated approach equips municipalities with critical insights for effective urban water management and planning |
| **Strengths and Limitations** | **Strengths:** Utilization of Open-Source Data, simplified and Step-by-Step Guidelines, permits an enhanced risk management. <br> **Limitations:** Data quality dependency, and enhanced technical skills requirements.|
| **Requirements  (Instruments Used)** | **Time:** Moderate to extensive, depending on the complexity. <br> **Skills:** GIS proficiency,knowledge of a programming language e.g. R<br> **Equipment:** Computers for data processing, ArcGis/QGIS and data analysis. <br> **Costs:** Moderate to Low. Main requirement is computing power |
| **Keywords** | Hydrometeorological Baseline Assessment, Reanalysis Data, Drought hazards indices, SPI, SPEI, VHI, VCI, TCI, Aridity Index (AI), Extreme Precipitation Events Indices, Flood Frequency Analysis |

## Tool Manual

### _a. Tool Oveview_

The “Insights for urban water management using open-source data” tool consists of four components, all of which rely on open-source data. These components can be used sequentially or individually, allowing end-users to focus on specific aspects of interest. Each component includes its own set of steps.

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 17.png" alt="Figure_17" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 17: Four key components that constitutes the "Insights for urban water management using open-source data" tool.</figcaption>
</figure>

### _b. Tool Usage Steps_

<img src="{{ site.baseurl }}/assets/Tookit_Figures/Insights_Pic1.png" alt="Insights_1" style="width: 100vw; height: auto; display: block; margin: 0 auto;" />

<img src="{{ site.baseurl }}/assets/Tookit_Figures/Insights_Pic2.png" alt="Insights_2" style="width: 100vw; height: auto; display: block; margin: 0 auto;" />

| **Advantages**                                                                 | **Limitations**                                                                 |
|--------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| Utilizes open-source data, making it accessible for municipalities with limited resources | Dependency on data quality of open-source datasets                             |
| Provides step-by-step guidelines for comprehensive watershed assessment       | Requires a minimum of technical skills, including proficiency in programming (e.g., R) |
| Enables data-driven decision making for local authorities                     | Does not provide access to all types of open-source data                        |
| Helps identify vulnerabilities and implement proactive measures               | May require significant time investment to conduct full assessment             |
| Applicable at multiple scales (urban and peri-urban areas)                    | Potential limitations in regional applicability                                |
| Incorporates visual tools to facilitate stakeholder communication             | Results may be limited by the resolution and coverage of available open data   |

## Study Case

The Prek Te watershed and Kratie village serve as the case study where the four components of 'Insights for Urban Water Management using Open-Source Data' were applied.

### 1.	Hydrometeorological baseline assessment

In this section, we showcase examples of the outputs generated by the provided R scripts.

<figure style="text-align: center;">
  <!-- Top full-width image -->
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 18_a.png" alt="Top Image" style="width: 100%; height: auto; margin-bottom: 0.5em;" />

  <!-- Bottom two half-width images -->
  <div style="display: flex; justify-content: center; gap: 1em;">
    <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 18_b.png" alt="Bottom Left" style="width: 48%; height: auto;" />
    <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 18_c.png" alt="Bottom Right" style="width: 48%; height: auto;" />
  </div>

  <figcaption>Figure 18: Examples of generated maps illustrating the multi-annual mean of precipitation (a), temperature (b) and potential evapotranspiration (c).</figcaption>
</figure>

<br>
<br>


<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 19_.png" alt="Figure_19" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 19: Spatial distribution of long-term mean monthly precipitation, temperature and potential evapotranspiration</figcaption>
</figure>


### 2.	Drought hazards assessment

### _a.	For Aridity Index (AI)_

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 20.png" alt="Figure_20" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 20: Temporal distribution of yearly Aridity Index in Prek Te watershed. The orange line represents the limit of humid climate values above this threshold means a dry-sub humid climate. The dashed blue line is the linear trend of the annual change in the aridity index.</figcaption>
</figure>

### _b.	For Standardized Precipitation Index (SPI) and Standardized Precipitation and Evapotranspiration Index (SPEI)_

The provided R script permits to calculate the SPI and SPEI over different time scales (1, 3, 6, 9, 12, 24 months) and to identify drought periods. 

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 21_a.jpg" alt="Figure 21_a" style="width: 100%; height: auto; margin-bottom: 0.5em;" />
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 21_b.jpg" alt="Figure 21_b" style="width: 100%; height: auto;" />
  <figcaption>Figure 21: Results of SPI and SPEI calculation using 12 months’ time scale. Red areas indicate drought periods.</figcaption>
</figure>

### _c.	For Vegetation Health Index (VHI)_

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 22.png" alt="Figure_22" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 22: Temporal distribution of VHI during the first quarter of the year between 2005-2022. Years with red coverage indicate agricultural drought periods.</figcaption>
</figure>

Based on the results illustrated in Figure 16, the Prek Te watershed (and Kratie village) experienced during the first quarter of the year in 2005, 2019, and 2020 drought conditions.

### 3.	Evaluating trends in precipitation extremes

In this section, we focus solely on R10 mm, one of the 13 calculated EPE indices, which showed a significant trend compared to the other indices in the Prek Te Watershed in Cambodia. 

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 23.png" alt="Figure_23" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 23: Temporal variation of R10 mm in Prek Te watershed in Cambodia between 1979-2024. Years with darker colors had higher number of days where daily precipitation exceeded 10mm</figcaption>
</figure>

<br>
<br>

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 24.png" alt="Figure_24" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 24: Regions within the Prek Te watershed that show a significant trend in R10mm. A trend is considered significant if the p-value is below 0.05.</figcaption>
</figure>

### 4.	Flood Frequency analysis

The Table 7 summarizes the expected flood magnitudes (in meters) for various return periods (in years); and Figure 25presents the flood frequency curve for the Kratie station showing the alignement between the selected distribution and the recorded data.

Table 7. Return Periods and Associated Flood Heights. 

| Return Period (Years) | Flood Magnitude (m) |
|-----------------------|---------------------|
| 2                     | 21.11               |
| 5                     | 22.26               |
| 10                    | 22.82               |
| 25                    | 23.35               |
| 50                    | 23.65               |
| 100                   | 23.88               |

<figure style="text-align: center;">
  <img src="{{ site.baseurl }}/assets/Tookit_Figures/Figure 25.png" alt="Figure_25" style="max-width: 100%; height: auto;" />
  <figcaption>Figure 25: Flood frequency curve of the Kratie station.</figcaption>
</figure>

**Analysis of Flood Frequency Analysis Results:**
The data indicates a clear trend in flood magnitudes as the return period increases. Notably: 
- The flood magnitude for a 2-year return period is estimated at 21.11 meters, while the magnitude for a 100-year return period rises to 23.88 meters. This increase highlights the growing risk associated with less frequent, more severe flooding events.
- The increments in flood magnitude between shorter return periods (e.g., from 2 to 5 years) are more pronounced, suggesting that even slight increases in frequency can lead to significant changes in expected water levels.
- As the return period extends, the increments in flood magnitude become smaller, indicating a diminishing rate of change for more extreme events


## Access to the tool

The tool can be accessed <a href="https://th-koeln.sciebo.de/s/pZGEHvJRJXlAleo" target="_blank" rel="noopener noreferrer">**here**</a>, along with the supporting documentation.

## Further Reading

Similar tool to assess drought hazards:<br>
•	SPI : <a href="https://drought.emergency.copernicus.eu/tumbo/gdo/map/" target="_blank" rel="noopener noreferrer">Global Drought Observatory</a><br>
•	SPEI: <a href="https://spei.csic.es/database.html" target="_blank" rel="noopener noreferrer">Global SPEI database</a><br>
•	SPI, SPEI, VHI: <a href="https://experience.arcgis.com/experience/883e8644b5ed4f029657565e24fe9968/" target="_blank" rel="noopener noreferrer">Global Drought Information System</a><br>
Similar tool for FFA: <a href="https://serc.carleton.edu/hydromodules/steps/168500.html" target="_blank" rel="noopener noreferrer">Guidelines Introduction to Flood Frequency Analysis</a>  
