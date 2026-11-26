---
layout: tool
title: "Groundwater Modeling System-GMS"
parent: Data Processing
grand_parent: D2D Toolbox
nav_order: 5
permalink: /toolbox/data-processing/groundwater-modeling-system-gms/
summary: "Graphical environment for building and running groundwater simulations, interfacing with MODFLOW, MT3DMS, MODPATH, PEST and other numerical models."
authors: "Lamees Abdulaziz"
year: "2019"
kind: software
topics: []
software: ["GMS", "MODFLOW", "MT3DMS", "MODPATH", "PEST"]
keywords: ["groundwater modeling", "flow and transport simulation", "particle tracking", "geostatistics"]
---

## Background

The Groundwater Modeling System (GMS) is a comprehensive graphical user environment for performing groundwater simulations. The entire GMS system consists of a graphical user interface (the GMS program) and a number of analysis codes (MODFLOW, MT3DMS, etc.). The GMS interface is developed by Aquaveo, LLC in Provo, Utah.

GMS was designed as a comprehensive modeling environment. Several types of models are supported and facilities are provided to share information between different models and data types. Tools are provided for site characterization, model conceptualization, mesh and grid generation, geostatistics, and post-processing.

More information [here](https://www.aquaveo.com/software/gms-groundwater-modeling-system-introduction).

## Principle

GMS includes a number of numerical models programs that are separate from GMS that are used to run an analysis on simulation. The simulation can be built in GMS, and then run through the numerical model program. GMS can then read in and display the results of the analysis.

The following numerical models are currently supported in GMS.

- MODFLOW (originally called the Modular Three-Dimensional Finite-Difference Ground-Water Flow Model) is a 3D, cell-centered, finite difference, saturated flow model developed by the United States Geological Survey (McDonald & Harbaugh, 1988). MODFLOW can perform both steady state and transient analyses and has a wide variety of boundary conditions and input options.
- MODPATH is a particle tracking code that is used in conjunction with MODFLOW. After running a MODFLOW simulation, the user can designate the location of a set of particles. The particles are then tracked through time assuming they are transported by advection using the flow field computed by MODFLOW. Particles can be tracked either forward in time or backward in time. Particle tracking analyses are particularly useful for delineating capture zones or areas of influence for wells. MODPATH was developed by the U.S. Geological Survey.

MT3DMS (Modular Transport, 3-Dimensional, Multi-Species model) is a modular three-dimensional transport model for the simulation of advection, dispersion, and chemical reactions of dissolved constituents in groundwater systems (Zheng, 1990). MT3DMS uses a modular structure similar to the structure utilized by MODFLOW. MT3DMS is used

- in conjunction with MODFLOWin a two-step flow and transport simulation.
- PEST (Parameter ESTimation) is a general purpose parameter estimation utility developed by John Doherty of Watermark Computing. The nonlinear parameterestimation algorithm used by PEST is uniquely robust and powerful have been developed for use with complex environmental models. The purpose of PEST is to assist in data interpretation, model calibration, and predictive analysis.
- PHT3D is a multicomponent transport model for three-dimensional reactive transport in saturated porous media developed and maintained by Henning Prommer and Vicent Post. PHT3D is a combination of MT3DMS and PHREEQC-2. The PHREEQC component allows for a variety of low temperature aqueous geochemical reactions.
- SEAWAT is a three-dimensional variable-density groundwater flow and transport model developed by the USGS based on MODFLOWand MT3DMS.
- SEAM3D (Sequential Electron Acceptor Model, 3D) is a reactive transport model used to simulate complex biodegradation problems involving multiple substrates and multiple electron acceptors. It is based on the MT3DMS code. SEAM3D was developed by Mark Widdowson at Virginia Tech University.
- MODAEM is an analytic element model developed by Vic Kelson of Wittman Hydro Planning Associates (WHPA) of Bloomington, Indiana. The model is defined by “analytic elements” representing line sources and sinks such as rivers and drains or specified head and specified flow boundaries. Wells are also represented as points, and recharge and aquifer properties can be defined as polygons. MODAEM then formulates a set of equations based on these entities and the equations can be solved for any location in the horizontal plane.
- UTEXASis a slope stability software package created by Dr. Stephen G. Wright of the University of Texas at Austin. UTEXAS is used to analyze slope stability using the limit equilibrium method. The user provides the geometry and shear strength parameters for the slope in question and UTEXAS4 computes a factor of safety against slope failure. The factor of safety for a candidate failure surface is computed as the forces driving failure along the surface divided by the shear resistance of the soils along the surface.
- SEEP2D is a two-dimensional steady-state finite element groundwater model developed by Fred Tracy of the Engineer Research and Development Center. Both saturated and unsaturated flow is simulated. SEEP2D is designed to be used on profile models (XZ models) such as cross-sections of earth dams or levees.
- FEMWATER (Finite Element Model of Water Flow Through Saturated-Unsaturated Media) model is a 3D finite element, saturated/unsaturated, density driven, flow and transport model. FEMWATER was originally written by G.T. (George) Yeh at Penn State University (Yeh, et. al., 1992). The version of FEMWATER that is supported by GMS has been modified by G.T. Yeh and Dr. Hsin-Chi (Jerry) Lin of the U.S. Army Engineer Waterways Experiment Station (WES).

T-PROGS (Transition PRObability GeoStatistical) software developed by Steven Carle. The T-PROGS software is used to perform transition probability geostatistics on borehole data. The output of the T-PROGS software is a set of N material sets on a 3D grid. Each of the material sets is conditioned to the borehole data and the materials proportions and transitions between the boreholes following the trends observed in the borehole data. These material sets can be used for stochastic simulations with MODFLOW.

## Manual

The limited open source version for GMS software can be downloaded from [here](https://www.aquaveo.com/downloads-gms) and more advanced versions for purchasing can be found [here](https://www.aquaveo.com/software/gms-pricing).

GMS manual can be found [here](http://gmsdocs.aquaveo.com/GMS_User_Manual_v10.3.pdf).

## Exercise

Step by step tutorials, videos and more can be found [here](https://www.aquaveo.com/software/gms-learning).

## Example

Samples of research, papers, publications, and other articles citing the Groundwater Modeling System (GMS) [here](https://www.aquaveo.com/software/gms-research-citations).
