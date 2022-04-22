---
date: 2019-02-19 15:05:15
description: 'Using EUSTACE temperature data for calibration or validation inclimate
  model research

  Introduction and background

  Climate models are always run for a historical period and (often) also for the future
  to get an idea of the climate change that we can expect. The quality of the projections
  for the future can only be determined indirectly, since we, of course, have no observations
  for the future. For the past we do have observations, therefore the climate model
  runs for the past are compared with the historical observations. The Global daily
  air temperature based on station and satellite data, 1850 on can also be used user
  for the historical temperature observations.'
layout: base_eustace
order: 0
permalink: /users/use-if-temperature-data/high-resolution-climate-modelling/
title: High resolution climate modelling
---

<h2><strong>Using EUSTACE temperature data for calibration or validation inclimate model research</strong></h2>
<h3><strong>Introduction and background</strong></h3>
<p>Climate models are always run for a historical period and (often) also for the future to get an idea of the climate change that we can expect. The quality of the projections for the future can only be determined indirectly, since we, of course, have no observations for the future. For the past we do have observations, therefore the climate model runs for the past are compared with the historical observations. The Global daily air temperature based on station and satellite data, 1850 on can also be used user for the historical temperature observations.</p>
<p></p>
<p><img height="267" src="https://www.eustaceproject.org/eustace/static/media/uploads/climate_model_grid.jpg" width="576"></p>
<p><b>Figure 1</b> Schematic presentation of a climate model: the earth is subdivided in many grids in horizontal and vertical direction: the climate model simulates the climate for each grid.</p>
<p>Climate models calculate the average of the climate variables over a grid (Figure 1). Grid size varies between climate models (Figure 2). In global climate models the spatial resolution is relatively coarse, although now also high resolution global simulations are under development with grid sizes of about 25 km (e.g. in the <em><strong><a href="https://www.primavera-h2020.eu/">PRIMAVERA project</a></strong></em>). Observational station data cannot be compared directly with the climate model data, since the station data give point measurements and the climate model give area average data. This is especially a problem for precipitation data (since some rainfall is very local), but also for temperature in a spatially heterogeneous area this may cause difficulties.</p>
<p></p>
<p><b><img height="227" src="https://www.eustaceproject.org/eustace/static/media/uploads/spatial_resolution_climate_models.png" width="500"></b></p>
<p><b>Figure 2</b> Evolution of spatial resolution in Global Climate Models used for IPCC assessment reports (Source: <a href="http://www.wmo.int/pages/themes/climate/climate_models.php">www.wmo.int/pages/themes/climate/climate_models.php</a>).</p>
<p></p>
<p> <img height="396" src="https://www.eustaceproject.org/eustace/static/media/uploads/eobs_ecad_satellite_temperature.png" width="600"></p>
<p><b>Figure 3</b><b> </b>Differences in spatial resolution based on different data sources (E-OBS: based on interpolation of station data from ECA&amp;D taking into account height) (Source: E. Good)</p>
<p> </p>
<p>Station data are only available for a limited number of locations, whereas climate models simulate the climate for a large region or the whole globe. To overcome this, the following approaches can be followed:</p>
<ul>
<li>Station data can be interpolated in a sophisticated way (e.g. taking into account the effect of height on temperature, or the effect of the presence of the sea or large water bodies). The resulting gridded datasets give estimates of the e.g. area average temperature in the past at locations where no observations took place. An example of such a dataset is the E-OBS data set (see also section 4.4 in the Product User Guide).</li>
<li>Another way to create a dataset with a better spatial coverage is the use of re-analysis. In reanalysis the climate in the past is simulated with a weather model integrating as much observational data as possible.</li>
<li>Use of satellite data. With satellites several climate variables can be measured, directly or indirectly. The advantage is the good spatial coverage and higher resolution (Figure 3). When measured indirectly the measured variable should be translated to the required climate variable. EUSTACE is an example of such a data set, where the measured surface skin temperature is translated to the air temperature.</li>
</ul>
<p>In climate models every grid is assigned a certain “surface”: land, sea, ice, etc. To assign a grid to a certain surface a “mask” is used (Figure 4). Although the grid size has decreased considerably in the past, it is still not exactly the same as in reality. In reality grids may contain two or more types of surfaces (e.g. land and ocean). The satellite observations used in EUSTACE are based on reality and in the project different methods are used to estimate the air temperature from the skin temperature above different surfaces. For a grid that contains in reality more than 1 type of surface, estimates of the air temperature for the various surfaces within that grid are made within EUSTACE. This is possible since the spatial resolution of the used satellite data is clearly higher than the final spatial resolution in the EUSTACE-data set (about 0.25˚).</p>
<p></p>
<p><b><img height="136" src="https://www.eustaceproject.org/eustace/static/media/uploads/mask_climate_data.png" width="600"></b></p>
<p><b>Figure 4</b> Left: hypothetical distribution of the “surfaces” ocean, land and ice over different grids. Right: a way to create a “mask” where only one surface is assigned to a grid cell (in this case land (green) is used in preference to ice (light blue) and ocean (blue), and ice is used in preference to ocean).</p>
<p> </p>
<h3><strong>How can the EUSTACE dataset be used in PRIMAVERA?</strong></h3>
<p>PRIMAVERA is working on high resolution global climate modelling. Several models will be run on a 0.25° spatial resolution and will be compared with model simulation with coarser resolutions, used until now. The idea behind this is that several processes may be simulated better due to the higher resolution. As part of the process of climate model development the model results are always validated. The currently available sources of data for the past-current climate do have some disadvantages:</p>
<ul>
<li>Interpolated station data: the E-OBS dataset is available from 1950 on, but it is available only for land and only for Europe. The dataset is available on a 0.25° spatial resolution and for determining the temperature per grid only the land surface is taken into account. Therefore grids with sea and land only give the average temperature for the area over land. Besides this, in regions with a lot of differences in height and land cover and a limited number of station data (an advantage is the availability of precipitation and sea level pressure).</li>
<li>Re-analysis: currently available global re-analyses often have a relatively coarse spatial resolution (<em><strong><a href="https://climatedataguide.ucar.edu/climate-data/atmospheric-reanalysis-overview-comparison-tables">https://climatedataguide.ucar.edu/climate-data/atmospheric-reanalysis-overview-comparison-tables</a></strong></em>).</li>
<li>Satellite based observational data sets: Until now these datasets were available for a limited period, the data were only available for a limited area and/or data were missing for days/periods with no measurements due to clouds. The EUSTACE project tries to overcome these shortcomings of satellite based data by creating a data set for all surfaces and using a sophisticated statistical method for filling in the days/period without data and for extrapolating to the past.</li>
</ul>
<p>During the development of the data file structure for the EUSTACE products, someone form the PRIMAVERA project was interviewed.  The final EUSTACE dataset is interesting to them since it will be a global dataset covering all surfaces, and since it has a high resolution (similar to the one they use for their highest resolution runs):</p>
<ul>
<li><b>Structure of the dataset: </b>Masks for land-water used in climate models are not the same as the real “masks”. This has to do with the modelling resolution (small island may not be explicitly included, Scandinavia may be connected with Denmark, etc.). Having estimates for air temperature for the different surfaces separately would allow them to make a dataset for validation with air temperatures for the same surfaces per grid cell as used in the climate model runs. This would allow them to make a better or “fairer” validation.</li>
<li><b>Use of uncertainty information:</b> For validation of climate model data it is important to have an idea of the uncertainty in “observations”: If there is wide variation in air surface “observations” (or estimates) then the simulated air temperature by the climate model may still be in the range of the “observations” although at first sight they may seem to differ a lot. This may clearly affect the conclusion about whether the climate model run has or does not have a (large) bias.</li>
</ul>
<p>Validation of climate model projections is done by comparing the statistics produced by the climate model with the statistics of the “observations” , e.g. for the average temperature in a month, or for the highest temperature reached per year.  In the final EUSTACE-dataset information is given on the uncertainty per day, but also an ensemble is produced to describe the uncertainty.  If one wants to take into account the uncertainty in the EUSTACE-dataset for validation of climate model projections, the  ensemble can be used best.</p>
<div>
<div>
<p></p>
</div>
</div>
