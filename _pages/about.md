---
layout: about
title: About
permalink: /
subtitle: "\"The mystery of life isn't a problem to solve, but a reality to experience.\" - Frank Herbert"

profile:
  align: right
  image: prof_pic_og.JPG
  image_circular: true # crops the image to make it circular
  more_info: >
    <p><a href='https://clasp.engin.umich.edu/'>University of Michigan</a> </p>
    <p>PhD Student in Climate Science</p>
    <p><a href="mailto:nandrosk@umich.edu">nandrosk@umich.edu</a></p>

news: false # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page
---

Since the summer of 2024, I have been a pre-candidate PhD student at the [University of Michigan's](https://clasp.engin.umich.edu/) Climate and Space Science department advised by Dr. Christiane Jablonowski. Currently, I am involved in the [NSF StormSPEED project](https://sites.google.com/umich.edu/nsf-stormspeed) which aims to implement an existing non-hydrostatic spectral element (SE) dynamical core from the Department of Energy (DOE) into NCAR's Community Earth System Model to enable cloud-permitting climate modeling for the entire globe. Modeling the climate at high resolutions (at the km-scale) requires extensive computational power, which makes it expensive to run ensemble simulations or single simulations for long time periods. This can make it difficult to tune the model to accurately represent phenomenon near the grid or sub-grid scale, like clouds and storm systems. 

<div style="display: flex; flex-direction: row; align-items: center; justify-content: center;">
    {% include figure.liquid loading="eager" path="assets/img/squall_radref_physical_scale.png" title="IR_Absorption_Profile" class="img-fluid rounded z-depth-1" %}
</div>
<div class="caption">
    The composite radar reflectivity for selected times 45 minutes (a), 90 minutes (b), 135 minutes (c), and 180 minutes (d) for an idealized squall line test case on a reduced radius Earth with a simple Kessler physics scheme. With a scale factor of 120 on the radius, a 1-degree cubed sphere grid (ne30) produces grid spacing of about 1 km. Each plot uses a Miller cylindrical projection. The squall is initialized analytically with 7 non-hydrostatic warm bubble perturbations each with a 5 km radius spaced 15 km apart on top of a hydrostatic and cyclostrophic background favorable for the formation of a squall line.
</div>

Idealized test cases can provide computationally efficient tools to probe the effectiveness of climate models and reveal physical insights on how we can improve the representation of important phenomenon. As a part of StormSPEED, I have been working on an idealized squall line test case to analyze how well cloud-permitting climate models, like the SE model from DOE, can represent moist convective dynamics at the km-scale, which is often referred to as the 'gray scale of convection' where some aspects of convection begin to be explicitly resolved (like deep convection) while other aspects still rely on subgrid parameterizations. How important parameterizations are at these scales and how existing physics parameterizations used at coarser resolutions should be adjusted at these resolutions are key open questions I seek to answer.

In 2024, I recieved my BS in Physics at [Cal Poly San Luis Obispo](https://calpoly.edu) with minors in mathematics and astronomy. My senior project focused on research I conducted at the [Center for Astrophysics](https://www.cfa.harvard.edu/facilities-technology/telescopes-instruments/parker-solar-probe) on ion cyclotron electromagnetic waves in the corona using NASA's Parker Solar Probe. At Cal Poly, I also worked on measuring stellar ages and identifying rare nuclear fission events. At UM, I have shifted my sights to understanding our atmosphere here on Earth through modeling and analyzing how they can be validated to achieve actionable and reliable projections.


Academic Interests:
* Model validation of high resolution climate models
* Ideal simulation test cases as tools for analyzing model biases, understanding physical processes, and teaching.
* Using environomental and demographic information to assess risk to environmental hazards at the community level
* Data visualization and interaction as an effective tool for teaching others
<br />
<br />
<br />
See your polynomial of the day:<br />

<iframe src="https://www.desmos.com/calculator/ibkd035vqz?embed" width="750" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>
