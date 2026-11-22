---
layout: default
title: "Simplified Surface Energy Balance (SSEB) model"
parent: Data Processing
grand_parent: D2D Toolbox
nav_order: 15
permalink: /toolbox/data-processing/simplified-surface-energy-balance-sseb-model/
---

# Simplified Surface Energy Balance (SSEB) model

*Posted 2018-06-21*

**Prepared by: Tran Thi Ha Van**

---

**1. Background**

- SSEB model was developed by Senay et al. (2007) to provide rapid estimates of actual evapotranspiration (ETa) over large areas
- SSEB is a promising tool for ETa mapping
- Minimal amount of ancillary data required
- Simple procedure, easier and less expensive to implement
- Best performance
- SSEB model can also quantify the spatial extent of irrigated fields, the actual crop water consumption & water-use dynamics.

 Table 1. Modeling and data characteristics of SSEB model

<table><tbody><tr><td><strong>SSEB model</strong>  </td></tr><tr><td>Modeling approach  </td><td>Remote sensing energy balance  </td></tr><tr><td>Target monitored/output  </td><td>Actual evapotranspiration (Eta)  </td></tr><tr><td>Spatial resolution  </td><td>Limited by thermal data:  <p>MODIS/AVHRR: 1km</p> <p>Landsat: 30m</p> </td></tr><tr><td>Spatial extent  </td><td>Global (potentially)  </td></tr><tr><td>Frequency of product  </td><td>Limited by thermal data:  <p>MODIS: 2 days</p> <p>Landsat: 16days</p> </td></tr><tr><td>Period of record  </td><td>Limited by thermal data:  <p>AVHRR: 1989 – current</p> <p>MODIS: 2000 – current</p> <p>Landsat: 1982 – current</p> </td></tr><tr><td>Geographic projection  </td><td>Latitude – longitude  </td></tr><tr><td>GIS environment  </td><td>Yes (ArcGIS)  </td></tr><tr><td>Description of product  </td><td>Best applied to irrigated systems  </td></tr><tr><td>Limitation for operational implementation  </td><td>Cloud cover and lack of climatic record  </td></tr></tbody></table>

---

**2. Principle**

The SSEB model maintains and extends the major assumption of SEBAL (Bastiaanssen et al., 1998) and METRIC (Allen et al., 2007) models. These two models assume that the difference between land surface temperature (LST) and air temperature varies linearly with LST. SSEB further assumes that the difference between LST and air temperature also varies linearly with ETa (Haynes and Senay, 2012). LST is used as a scalar to indicate the water availability of the pixel by assuming that the hot extreme pixel is located in a dry, bare area with no ET and the cold extreme pixel is located in a well-vegetated field with the maximum ET.

![]({{ site.baseurl }}/assets/uploads/2018_06_van5-530x414.jpg)

                                      Figure 1: ETa estimation based on SSEB equation

Using ArcGIS tool “Raster Calculator” and the software “ETo Calculator” (developed by FAO) to calculate relevant variables.

<http://www.fao.org/land-water/databases-and-software/eto-calculator/en/>

[*How Raster Calculator works*](http://desktop.arcgis.com/en/arcmap/10.3/tools/spatial-analyst-toolbox/how-raster-calculator-works.htm)

According to Al Zayed et al. (2016), SSEB is performing best in comparison to the SEBAL, METRIC & MOD16A2. The result from the research of Lian and Huang (2015) indicated that the instantaneous latent heat fluxes estimated by SSEB model have a good correlation with values measured by eddy covariance flux tower (EC) (R2 = 0.90). Bezerra et al. (2015) emphasized that the SSEB model will be a promising tool for the area where the ground data is rare. The Landsat-based SSEB ETa model was validated successfully by Gowda et al. (2009) using lysimeter data in Bushland, Texas. It is one of the most simplified approaches for mapping ETa.

---

**3. Manual**

![]({{ site.baseurl }}/assets/uploads/2018_06_van6.jpg)
*Figure 2: SSEB approach for ET estimation*

- The selection of the satellite images takes into account the Cloudiness in the research area during the satellite pass. Landsat image pre-processing is necessary. Free Satellite Imagery Data Sources: <https://gisgeography.com/free-satellite-imagery-data-list/>
- The SSEB approach for ETa estimation includes 3 different components: the land surface temperature (LST), Normalize Different Vegetation Index (NDVI), and reference ET (ETo). The ETo calculator assesses ETo from meteorological data by means of the FAO Penman-Monteith equation.
- Assessment criteria for validation of this model are:
- Water balance
- Daily NDVI value vs daily ETa

Integrated NDVI (iNDVI) vs seasonal ETa

![]({{ site.baseurl }}/assets/uploads/2018_06_van1-530x275.jpg)
*Figure 3: Flowchart of the computational steps of SSEB algorithm*

- Get TH and TC

Methods for selecting proper hot and cold pixels are described by Allen et al., (2002). Accordingly, the cold pixel is the pixel with minimum Tx and maximum NDVI (***e.g. the field/crop, natural vegetation cover…***). And the hot pixel is the pixel with maximum Tx and minimum NDVI (***e.g. bare soil, urban area…***).

![]({{ site.baseurl }}/assets/uploads/2018_06_van2-530x369.jpg)
*Figure 4: Comparing NDVI and LST to define hot and cold pixels*

- Use” Raster Calculator” to get ETf
- Use ET0 Calculator for estimating ETo for the satellite image

Utilize again “Raster calculator” to get ETa by multiply ETf by 1.2 ETo

---

**4. Exercise**

**Estimating ETa for Rahad Irrigated Scheme following SSEB Method**

**Retrieving Data:**

- Satellite image - Landsat 8
- Source: U.S. Geological Survey through Earth Explorer <http://earthexplorer.usgs.gov>
- Geographical information - Path: 172 & Row: 50
- Date acquired: 2013-10-26

![]({{ site.baseurl }}/assets/uploads/2018_06_van3-530x686.jpg)

![]({{ site.baseurl }}/assets/uploads/2018_06_van4-530x686.jpg)

Link of exercise and relevant data: <https://drive.google.com/open?id=1EoH4Dj6uv2wGaheWRxxbBewwjBOiapXt>

---

**5. Example**

- **Water Productivity Mapping (WPM) Using Landsat ETM+ Data for the Irrigated Croplands of the Syrdarya River Basin in Central Asia**

(Platonov et al., 2008)

To address the better land and water management for the Syrdarya river basin of Central Asia, the study used time-series Landsat ETM+ data to produce WPMs of irrigated cotton fields. Water use by crops (actual evapotranspiration) mapping is based on SSEB model.

- **Remote Sensing Based Actual Evapotranspiration Mapping for Drought Monitoring and Water Budget Analysis**

Remote sensing and hydrologic modeling can provide globally

consistent and locally relevant data and information for:

- drought early warning
- planning and designing irrigation systems

ETa mapping is produced using the Operational Simplified Surface Energy Balance (SSEBop) model. The SSEBop setup is based on SSEB approach with unique parameterization for operational applications.

- **Satellite-based evapotranspiration over Gezira Irrigation Scheme, Sudan: A comparative study**

Understanding the spatio-temporal variation of ETa over irrigated agricultural areas helps to manage water. Evaluate the performance of four RS methods (SEBAL, SSEB, METRIC  & MOD16A2 models) for estimating ETa.

---

**6.Reference:**

Al Zayed, I.S., Elagib, N.A., Ribbe, L., Heinrich, J., 2016. Satellite-based evapotranspiration over Gezira Irrigation Scheme, Sudan: A comparative study. Agric. Water Manag. 177, 66–76. https://doi.org/10.1016/j.agwat.2016.06.027

Allen, R., Waters, R., Tasumi, M., Trezza, R., Bastiaanssen, W., 2002. SEBAL Surface Energy Balance Algorithms for Land —Advance Training and User’s Manual.

Allen, R.G., Tasumi, M., Trezza, R., 2007. Satellite-Based Energy Balance for Mapping Evapotranspiration With Internalized Calibration ( METRIC ) – Model. J. Irrig. Drain. Eng. 133, 380–394. https://doi.org/10.1061/(ASCE)0733-9437(2007)133

Bezerra, B.G., Silva, B.B. da, Santos, C.A.C. dos, Bezerra, J.R.C., 2015. Actual Evapotranspiration Estimation Using Remote Sensing: Comparison of SEBAL and SSEB Approaches. Adv. Remote Sens. 4, 234–247. https://doi.org/10.4236/ars.2015.43019

Gowda, P.H., Senay, G.B., Howell, T.A., Marek, T.H., 2009. Lysimetric evaluation of Simplified Surface Energy Balance approach in the Texas High Plains. Appl. Eng. Agric. 25, 665–670.

Haynes, J. V., Senay, G.B., 2012. Evaluation of the Relation between Evapotranspiration and Normalized Difference Vegetation Index for Downscaling the Simplified Surface Energy Balance Model. USGS Groundw. Resour. Progr. Eval.

Lian, J., Huang, M., 2015. Comparison of three remote sensing based models to estimate evapotranspiration in an oasis-desert region. Agric. Water Manag. 165, 153–162. https://doi.org/10.1016/j.agwat.2015.12.001

Platonov, A., Thenkabail, P.S., Biradar, C.M., Cai, X., Gumma, M., Dheeravath, V., Cohen, Y., Alchanatis, V., Goldshlager, N., Ben-Dor, E., Vithanage, J., Manthrithilake, H., Kendjabaev, S., Isaev, S., 2008. Water productivity mapping (WPM) using landsat ETM+ data for the irrigated croplands of the Syrdarya river basin in Central Asia. Sensors 8, 8156–8180. https://doi.org/10.3390/s8128156

Senay, G.B., Budde, M., Verdin, J.P., Melesse, A.M., 2007. A coupled remote sensing and simplified surface energy balance approach to estimate actual evapotranspiration from irrigated fields. Sensors 7, 979–1000. https://doi.org/10.3390/s7060979
