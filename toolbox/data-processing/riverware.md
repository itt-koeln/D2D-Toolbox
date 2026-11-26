---
layout: tool
title: "RiverWare"
parent: Data Processing
grand_parent: D2D Toolbox
nav_order: 14
permalink: /toolbox/data-processing/riverware/
summary: "Generalized river and reservoir simulation software for modelling water allocation, with pure, rule-based, and optimization run modes."
authors: "Mohammed Basheer"
year: "2018"
kind: software
topics: ["Water allocation modelling"]
software: ["RiverWare"]
keywords: ["water allocation modelling", "reservoir simulation", "rule-based simulation", "river systems"]
---

*Posted 2018-06-18* · Category: Water allocation modelling

![]({{ site.baseurl }}/assets/uploads/2018_06_riverware.png)

### 1. Background

RiverWare is a generalized river and reservoir simulation software that simulates water allocation and was developed by the Centre for Advanced Decision Support for Water and Environmental Systems (CADSWES) of the University of Colorado. With time steps ranging from one hour to one year, RiverWare can simulate hydrologic and hydraulic processes of several kinds of objects such as storage reservoirs, river reaches, diversion structures, and canals.

Modeling a river system using RiverWare requires knowing water supply and demand volumes. Therefore, links between RiverWare and water supply modelling tools (e.g. HEC-HMS, HBV, SWAT) and water demand modelling tools (such as CropWat) should be established.

References:

Zagona, E., Fulp, T., Shane, R., Magee, T. and Morgan, H. (2001) ‘Riverware: a Generalized Tool for Complex Reservoir System Modeling’, Journal of the American Water Resources Association, 37(4), pp. 913–929.

## Principle

Mass conservation represents the basis of modeling basic physical prosses of all objects in RiverWare. Additionally, more detailed physical processes are available for which the user may select a particular method of solution.

The rule-based simulation of RiverWare provides the ability to simulate the operation policies of river systems using logical statements rather than embedded logic for operations. Additionally, the Multiple Run Management (MRM), a utility that RiverWare has, provides the ability to run a model using combinations of stochastically generated hydrologic inputs and system operation policies.

## Manual

The Riverware source file can be downloaded from CADWES website (<http://cadswes2.colorado.edu/downloads/riverware/releases/>) and can be installed straightforward (<http://riverware.org/PDF/RiverWare/online-user-guides/rw-install-guide-windows.pdf>). However, a license is required to use the tool. Basic data required to develop a RiverWare model include river flow, water demand, system operation policies, reservoir data, and river reaches data. The amount of additional data required depends on the mathematical models selected to simulate the physical processes.

RiverWare presents the user with a palette of basic graphical icons representing features of a river basin objects. Each object contains the data structures, called slots, required for modeling processes on that object. Each object can be connected with other objects and afterwards, the model can be run in one of three modes: pure simulation, rule-based simulation, or optimization.

## Exercise

A full rule-based simulation model developed using RiverWare is attached in the following [link](https://th-koeln.sciebo.de/s/7GvM8phTer1IyZ2). The attachment includes the model file, the operation rules file, and the model description document.

This exercise gives an idea about the abilities of RiverWare in simulating complex river systems.

## Example

RiverWare has been used in modelling the impacts of the Grand Ethiopian Renaissance Dam on the Eastern Nile system. A publication on this study is available for free under the following link:

<http://www.tandfonline.com/doi/abs/10.1080/02508060.2016.1177698>
