---
layout: page
title: Idealized Modeling Hierarchy for Non-hydrostatic Dynamical Cores
description: Applying idealized test cases to understand how global climate models at the km-scale represent convection.
img: assets/img/squall_zoomed_in.png
importance: 1
category: work
related_publications: false
---

My current PhD research focuses on using a hierarchy of idealized test cases with increasing complexity to understand how climate models at the km-scale represent convection. My focus lies on the dynamical core, the component of an atmospheric model that solves the resolved equations of motion for fluid flow, and how it couples to the physics, the component that parameterizes processes not resolved by the discrete grid used by the model. I work within the Community Earth System Model (CESM) developed by the National Center for Atmospheric Research (NCAR) and on the [NSF StormSPEED project](https://sites.google.com/umich.edu/nsf-stormspeed) which aims to implement an existing non-hydrostatic spectral element (SE-NH) dynamical core from the Department of Energy (DOE) into CESM. I use the two non-hydrostatic dynamical cores within CESM, SE-NH and MPAS (Mesoscale Prediction Across Scales), to understand how the decisions made within the dynamical core affect convection at kilometer horizontal scales. 

# Table of contents
1. [Non-hydrostatic Dynamics and Convection](#introduction)
2. [The Non-hydrostatic Dynamical Cores in CESM](#paragraph1)
3. [An Idealized Modeling Hierarchy for Convection](#paragraph2)
4. [Snapshots of My Current Work](#paragraph3)
5. [Future Work](#paragraph4)
6. [Qualifying Exam Report](#paragraph5)

<a name="introduction"></a>
<br>
# Non-hydrostatic Dynamics and Convection

Global climate models have historical operated at resolutions above 25 km or more. At these coarse resolutions, the vertical pressure gradient force and gravity balance each other to good approximation. This 'hydrostatic approximation' has been a mainstay in climate modeling, embedded into the design of the dynamical core and physics components of atmospheric models. However, within the past decade global climate models have moved begun to reach scales on the order of kilometers (i.e. the km-scale). At these scales, the deviations from hydrostatic balance become important especially for convective storm systems and using non-hydrostatic equations of motion is key for representing these dynamics.

Convection is the vertical – often turbulent – transport of moisture and heat induced by buoyancy.

<a name="paragraph1"></a>
<br>
# The Non-hydrostatic Dynamical Cores of CESM

<details>
<summary><big><b>The Model Details</b></big></summary>
<br>

<ul>  
<li> NCAR’s Community Earth System Model <a href="https://www.cesm.ucar.edu/models/cesm2">(CESM)</a></li>
<li> <a href="https://www.cesm.ucar.edu/models/simple/aquaplanet">Aquaplanet Configuration</a> with Prescribed SSTs (QPC4)</li> 
<li> Community Atmosphere Model (CAM) Version 4 <a href="https://www2.cesm.ucar.edu/models/ccsm4.0/cam/">(user guide and a detailed scientific description available here)</a></li>
<li> Spectral Element Dynamical Core </li>
<li> 2-Degree Horizontal Resolution </li>
<li> 72 Level Vertical Resolution with Model Top at 0.1 hPa (~60 km) </li>
<li> 10 year simulations with monthly mean output: Only the last 5 years are used in time-averages. </li>
<li> Analytic moist baroclinic wave initial conditions (<a href = "https://www.cesm.ucar.edu/models/simple/fkessler"> moist_baroclinic_wave_dcmip2016</a> based on <a href = "https://doi.org/10.1002/qj.2241">Ullrich et. al 2014</a>) </li>
</ul>

</details>


<br>
<br>

<a name="paragraph2"></a>
<br>
# An Idealized Modeling Hierarchy for Convection
Idealized test cases can provide computationally efficient tools to probe the effectiveness of climate models and reveal physical insights on how we can improve the representation of important phenomenon. As a part of StormSPEED, I have been working on an idealized squall line test case to analyze how well cloud-permitting climate models, like the SE model from DOE, can represent moist convective dynamics at the km-scale, which is often referred to as the 'gray scale of convection' where some aspects of convection begin to be explicitly resolved (like deep convection) while other aspects still rely on subgrid parameterizations. How important parameterizations are at these scales and how existing physics parameterizations used at coarser resolutions should be adjusted at these resolutions are key open questions I seek to answer.


<br>
<br>

<a name="paragraph3"></a>
<br>
# Snapshots of My Current Work

<a name="paragraph4"></a>
<br>
# Future Work
List sensitivities here:


<a name="paragraph5"></a>
<br>
# The Full Report
If you're interested in learning more about my work, I wrote a full report for my qualifying exam in May 2026 that includes more figures and details, particularly on the squall line test case. You can access the report below:

<object data="https://nandroski.github.io/assets/pdf/Stratospheric_Ozone__CLIMATE_473_Project_Report.pdf" type='application/pdf' width="100%" height="500" align="middle">
  alt : <a href="https://nandroski.github.io/assets/pdf/Stratospheric_Ozone__CLIMATE_473_Project_Report.pdf">Stratospheric_Ozone__CLIMATE_473_Project_Report.pdf</a>
</object>

If the PDF does not render, you can access the report at the following link: [Stratospheric_Ozone__CLIMATE_473_Project_Report.pdf](https://nandroski.github.io/assets/pdf/Stratospheric_Ozone__CLIMATE_473_Project_Report.pdf)

<!-- <iframe src="https://nandroski.github.io/assets/pdf/Stratospheric_Ozone__CLIMATE_473_Project_Report.pdf" width="100%" height="500"> -->



