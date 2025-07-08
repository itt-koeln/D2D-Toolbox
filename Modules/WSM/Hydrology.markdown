---
layout: page
title: Hydrometeorology
permalink: /Hydrometeorology/
parent: Watershed Management
nav_order: 3
---

# Hydrometeorology

### 1- Water Balance:
The water balance is a fundamental hydrological tool that quantifies the movement and storage of water within a defined system (e.g., a catchment). It operates on the principle of mass conservation, ensuring all water inputs, outputs, and storage changes are accounted for. , meaning that for a
specific period of time (e.g., month, year or mean annual), the water inflows are equal to
the water outflows plus or minus any change of storage within the specified hydrological
unit (European Commission, 2015).




The water balance can be used to:
•
Assess the current status and trends in key hydrological components
•
Understand the importance of key hydrologic variables over diverse regions
•
Strengthen water management through evidence based decision making
•
Forecast flow (related to infrastructural design)



<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Water Balance: Advantages and Limitations</title>
    <style>
        table {
            width: 100%;
            border-collapse: collapse;
            margin-bottom: 20px;
        }
        th, td {
            padding: 10px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }
        th {
            background-color: #f2f2f2;
        }
    </style>
</head>
<body>

<h2>Water Balance: Advantages and Limitations</h2>

<table>
    <thead>
        <tr>
            <th>Key Advantages</th>
            <th>Major Limitations</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><strong>Holistic Understanding</strong><br>
                Provides a comprehensive view of water flow systems and resource distribution within a catchment.</td>
            <td><strong>Data Uncertainties</strong><br>
                - Spatial/temporal variability in precipitation (P), evaporation (E), and runoff (Q) measurements.<br>
                - Difficulties in quantifying the storage term (ΔS), especially for groundwater.</td>
        </tr>
        <tr>
            <td><strong>Implementation Simplicity</strong><br>
                Straightforward to apply under steady-state conditions (long-term averages) where storage changes (ΔS) can be neglected.</td>
            <td><strong>Practical Constraints</strong><br>
                - Less reliable in human-impacted basins (e.g., with dams, irrigation, or interbasin transfers).<br>
                - Limited applicability in data-scarce regions due to dependency on robust input datasets.</td>
        </tr>
        <tr>
            <td><strong>Component Estimation</strong><br>
                Enables derivation of unknown variables (e.g., calculating evaporation as \( E = P - Q \) when direct measurements are unavailable).</td>
            <td></td>
        </tr>
    </tbody>
</table>

<p><strong>Pro Tip:</strong> Combine with remote sensing (e.g., GRACE for ΔS) to mitigate limitations in ungauged basins.</p>

</body>
</html>

## Manual:

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Water Balance Equation</title>
    <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
    <script id="MathJax-script" async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/3.2.0/es5/tex-mml-chtml.js"></script>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        h2 {
            margin-bottom: 20px;
        }
        ul {
            margin-top: 0;
        }
    </style>
</head>
<body>

<h2>Water Balance Equations</h2>

<p>The water balance principle can be represented in two forms:</p>

<p>
  1. General Form: <br>
  \[
  \text{Inputs} = \text{Outputs} \pm \frac{dS}{dt}
  \]
</p>

<p>
  2. Detailed Hydrological Form: <br>
  \[
  P = R + E \pm \frac{dS}{dt}
  \]
  Where:
  <ul>
      <li><strong>P</strong> = Precipitation: The total water received as rain, snow, sleet, etc.</li>
      <li><strong>R</strong> = Runoff: Water that flows over the surface into streams, rivers, and lakes.</li>
      <li><strong>E</strong> = Evapotranspiration: The sum of evaporation from the land surface plus transpiration from plants.</li>
      <li><strong>\(\frac{dS}{dt}\)</strong> = Change in Storage: The rate of change in stored water, including surfaces such as wetlands, snowpacks, soils, and aquifers.</li>
  </ul>
</p>

<p>These equations are fundamental in hydrology for assessing water availability and planning resources in various geographic and climatic contexts.</p>

</body>
</html>

The simple water balance equation comprises the following four components:

1. **P** – Refers to solid and liquid precipitation.

2. **R** – Consists of:
   - Surface runoff (\( R_s \))
   - Subsurface runoff (\( R_{\text{sub}} \))
   - Groundwater runoff (\( R_{\text{gw}} \))

3. **E** – Can be decomposed into:
   - Surface evaporation (\( E_s \))
   - Interception (\( E_i \))
   - Unsaturated zone evaporation (\( E_u \))
   - Transpiration (\( E_t \))

4. **\(\frac{dS}{dt}\)** – Decomposed changes:
   - Surface storage change (\( \frac{dS_s}{dt} \))
   - Interception storage change (\( \frac{dS_i}{dt} \))
   - Unsaturated zone storage change (\( \frac{dS_u}{dt} \))
   - Groundwater storage change (\( \frac{dS_{\text{gw}}}{dt} \))

## Fundamental Assumptions of the Water Balance

The water balance approach typically relies on several key assumptions for its calculations:

- **Closed system**: Assumes no external water transfers are occurring unless they are explicitly modeled within the system.

- **Stationarity**: Assumes the model is valid for long-term averages. For short-term assessments, changes in storage (ΔS) must be considered.

- **Data integrity**: Relies upon accurate and reliable measurements of precipitation (P), evapotranspiration (E), and runoff (Q).
## Data Sources

- Public domain data
- Research data

## Tools

- Hydrological models
- Data analysis tools