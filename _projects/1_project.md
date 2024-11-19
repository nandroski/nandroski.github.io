---
layout: page
title: Climate and Stratospheric Ozone
description: Using CESM models to assess the effect of stratospheric ozone on the climate.
img: assets/img/OzoneFrac.png
importance: 1
category: work
related_publications: false
---

For my CLIMATE 473 Climate Physics course, I used an aquaplanet model to simulate how increases and decreases in stratospheric ozone can impact the climate system. 

The Theory of Ozone in the Atmosphere:
* Shortwave Interaction: UV absorption and oxygen photochemistry
* Longwave Interaction: Absorption bands and the atmospheric window

Model info:
See the full details in the user_namelist file at the bottom of the page
* Aquaplanet with prescribed sea surface temperatures
* Spectral Element dynamical core with CAM4 physics at 2 degree resolution
* 72 vertical level configuration (model top at about 0.1 hPa (65 km))
* Moist baroclinic wave initial conditions
* Prescribed ozone concentration (0.25X, 1X, 4X)
* 10 year long run with monthly mean output
* Gravity waves by orography are disabled

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Equatorial_Tprofile_O3comparison.png" title="Equatorial T Profile" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/MidLat_Tprofile_O3comparison.png" title="MidLatitude T Profile" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Polar_Tprofile_O3comparison.png" title="Polar T Profile" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Characteristic temperature profiles for 0.25X, 1X, and 4X ozone concentrations at the equator and at the poles. Each profile is a 5 year zonal average additionally meridionally averaged over 10 degrees of latitude to produce a profile characteristic of the region.
</div>