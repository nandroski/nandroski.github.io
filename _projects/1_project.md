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

# The Radiative Properties of Ozone:

Stratospheric ozone, despite it's relatively small concentration compared to other gases in the atmosphere, has a large influence on the climate on Earth. Ozone in the stratosphere is primarily responsible for the existence of a tropopause, where lapse rate of temperature switches sign and separates the unstably stratified troposphere from the stably stratified stratosphere. Ozone has strong interactions with both shortwave (SW) and longwave (LW) radiation.

<div class="row justify-content-sm-center">
    {% include figure.liquid loading="eager" path="assets/img/IR_AbsorptionBandHartmann.jpg" title="IR_Absorption_Profile" class="img-fluid rounded z-depth-1" %}
</div>
<div class="caption">
    Figure 1: Infrared absorption spectrum for key molecules in Earth's atmosphere. Obtained from Figure 3.4 in <a href = "https://doi.org/10.1016/B978-0-12-328531-7.00003-7"> Hartmann, D. (2016)</a>, created by <a href = "https://www.osti.gov/biblio/6546426"> Valley, S. L. (1965).</a>
</div>

Light at UV wavelengths in the stratosphere are absorbed by molecular oxygen (O2) and by ozone (O3) itself. The absorption by O2 is essential in the creation of ozone while the absorption of O3 is a key destructive process of ozone. In an oxygen rich atmosphere like Earth's, the concentration of ozone in the stratosphere is largely a balance between these photochemical creation and destruction processes. These reactions create a continuum absorption band of UV radiation between around $$200-300\text{ nm}$$.

Additionally, ozone has a strong vibration-rotation absorption band around $$9.6~\mu\text{m}$$ which lies in Earth's atmospheric window shown in Fig. 1. The atmospheric window is a region on the infrared spectrum between 8 to 13 $$\mu\text{m}$$ where the atmosphere is relatively transparent due to a lack of molecules with absorption bands here. However, since ozone's infrared absorption line lies within this window, changes in ozone concentration can strongly influence how transparent the window is and importantly how much radiation at these wavelengths escapes out to space.

# The Aquaplanet Model

An aquaplanet simulation is an idealized global atmospheric model that is completely water-covered with no land, topography, or sea ice. Aquaplanets use a data ocean, an ocean model that uses data to force and determine its state. In the Community Earth System Model (CESM), data-oceans come in two forms: a pure data model based an prescribed sea surface temperatures (SSTs) or a slab-ocean model where bottom heat flux and boundary layer depths are supplied to update SSTs  based on atmosphere-ocean fluxes. Additionally, while aquaplanets maintain a diurnal cycle, a perpetual equinox with a perfectly circular orbit (eccentricity and obliquity of zero) is enforced, resulting in no seasonal cycle. Aquaplanets provide a bridge in the hierarchy of atmospheric general circulation models between simplified physics component sets like the Held-Suarez configuration and Earth-like simulations used in the Atmospheric Modeling Intercomparison Project (AMIP). 

<div class="row justify-content-sm-center">
    {% include figure.liquid loading="eager" path="assets/img/OzoneFrac.png" title="ozone_distribution" class="img-fluid rounded z-depth-1" %}
</div>
<div class="caption">
    Figure 2: Zonally uniform ozone distribution for the 1×O3 control run based upon the AquaPlanet Experiment project specifications created by an annual average of the monthly AMIP ozone climatology. 
</div>

For this project, I ran **three** 10 year-long, fixed SST aquaplanet simulations with prescribed ozone concentrations. The first is a control ozone simulation $$(1\times\text{O3})$$, shown in Fig. 2, with a zonally-uniform, time-independent ozone distribution based upon the Aquaplanet Experiment Project standards that is based upon AMIP climatologies. In order to observe how increases and decreases to ozone impact climate, the other two runs apply a $$4\times$$ and $$1/4\times$$ factor to the $$1\times\text{O3}$$ control run respectively. For more details see the dropdowns below:

<details>
<summary>The Model Details</summary>
<br>

<ul>  
<li> NCAR’s Community Earth System Model <a href="https://www.cesm.ucar.edu/models/cesm2">(CESM)</a></li>
<li> <a href="https://www.cesm.ucar.edu/models/simple/aquaplanet">Aquaplanet Configuration with Prescribed SSTs (QPC4)</a> </li>
<li> Community Atmosphere Model (CAM) Version 4 <a href="https://www2.cesm.ucar.edu/models/ccsm4.0/cam/">(user guide and a detailed scientific description available here)</a></li>
<li> Spectral Element Dynamical Core </li>
<li> 2-Degree Horizontal Resolution </li>
<li> 72 Level Vertical Resolution with Model Top at 0.1 hPa (~60 km) </li>
<li> 10 year simulations with monthly mean output: Only the last 5 years are used in time-averages. </li>
<li> Analytic moist baroclinic wave initial conditions (<a href = "https://www.cesm.ucar.edu/models/simple/fkessler"> moist_baroclinic_wave_dcmip2016</a> based on <a href = "https://doi.org/10.1002/qj.2241">Ullrich et. al 2014</a>) </li>
</ul>

</details>

<details>
<summary>Do Ocean Gyres Occur on an Aquaplanet?</summary>
<br>

In class, we briefly discussed whether or not a planet without land, like an aquaplanet, would have ocean gyres. With a prescribed SST data-ocean, this question cannot be studied by the simulations run for this project as there is no explicit modeling of the ocean circulation. However, this analysis is possible for slab-ocean aquaplanet models. The authors <a href = "https://doi.org/10.1175/JCLI3874.1">Smith et. al (2006)</a> conducted a study that addresses this very question. In the study, they conducted three coupled ocean-atmosphere slab-ocean aquaplanet-like experiments on a low-resolution version of the Fast  Ocean, Rapid Troposphere Experiment (FORTE) model. The first configuration was a typical aquaplanet (WaterWorld) with no land or topography, the second an aquaplanet that contained a low barrier that blocks zonal flow in the ocean at all latitudes (RidgeWorld),and third an aquaplanet with a meridional barrier with a gap in the Southern hemisphere that allows circumglobal flow (DrakeWorld).
</details>

# Atmospheric Circulation

In the simulations, there are five key observations atmospheric circulation for higher ozone concentrations $$(4\times\text{O3})$$:
* Stratospheric warming
* Thicker stratosphere (higher stratopause and lower tropopause)
* An unchanged lower tropospheric lapse rate
* Strenghtened polar stratospheric jets
* Weakened Hadley Circulation

The opposite story is observed at lower ozone concentrations $$(1/4\times\text{O3})$$:
* Stratospheric cooling
* Thinner stratosphere (lower stratopause and higher tropopause)
* An unchanged lower tropospheric lapse rate
* Weakened polar stratospheric jets
* Strengthened Hadley Circulation

<div class="row">
    {% include figure.liquid loading="eager" path="assets/img/MidLat_Tprofile_O3comparison.png" title="Midlat T Profile" class="img-fluid rounded z-depth-1" %}
</div>
<div class="caption">
    Characteristic temperature profiles for 0.25X, 1X, and 4X ozone concentrations at mid-latitudes. Each profile is a 5 year zonal average that is meridionally averaged over 10 degrees of latitude between 40-50 degrees north to produce a profile characteristic of the mid-latitudes.
</div>


# Energy Balance

The radiative heating profiles of the $$1\times\text{O3}$$ aquaplanet depict the two key energy balances in the lower atmosphere: a stratosphere in radiative equilibrium and a troposphere in radiative-convective equilibrium. In the stratosphere, the longwave cooling matches the shortwave warming. On the other hand, the troposphere is radiatively cooling which offsets the convective heating from the surface.

For higher ozone concentrations $$(4\times\text{O3})$$ we see key observations on the radiative heating profiles:

* The LW and SW heating in the stratosphere increase in magnitude
* The LW and SW budgets in the troposphere are largely unaffected

For lower ozone concentrations $$(1/4\times\text{O3})$$ we again see the opposite in the stratosphere:
* The LW and SW heating in the stratosphere decrease in magnitude
* The LW and SW budgets in the troposphere are largely unaffected

On the global scale, a stable Earth-atmosphere climate system is in a balance between the incoming solar energy and the outgoing longwave radiation from Earth. Stable is meant in the sense that the climate system is at some equilibrium global average temperature over long time scales. This balance is called the top-of-atmosphere (TOA) balance. It is determined by the amount of solar radiation emitted by the Sun incident on Earth, the planetary albedo, and the outgoing longwave radiation. For our simulations, Earth's orbital distance and solar luminosity are constants.

The greater longwave cooling at higher ozone concentrations is a natural consequence of a warmer stratosphere caused by the greater solar absorption from ozone. We might then expect that the greater longwave radiation in the stratosphere would ultimately cause more outgoing longwave radiation at the top of atmosphere. Indeed, as Fig. shows, this is the case and at lower ozone concentrations we analogously see lower OLR on average. To maintain TOA balance, we should expect a decrease in planetary albedo with increasing ozone concentration.

The aquaplanet is a largely cloud covered world with vertically averaged cloud fractions between 0.70 and 0.95 across all the simulations. Clouds play an important role in the radiative budget of the atmosphere because of their shortwave albedo effects and their longwave, greenhouse effects. The albedo effects are particularly important for aquaplanets without sea ice because clouds provide the only mechanism for planetary albedo to change from the oceanic albedo across the globe. We see that the inverse relationship between global cloud cover and ozone concentration is a result of the top-of-atmosphere radiative balance between solar absorption and outgoing long wave radiation. In the $$4\times\text{O3}$$ run, we see that a decrease in global cloud cover causes a decrease in planetary albedo (greater solar absorption) that offsets that greater OLR to maintain the top of atmosphere radiative balance.

# Quasi-Biennial Oscillation




# Future Work and Questions


# The Full Report
If you're interesting in learning more about this project, I wrote a full report for my course project that includes more figures and details. You can access the report below:

