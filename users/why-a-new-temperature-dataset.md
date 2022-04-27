---
date: 2019-02-19 15:28:11
description: "Currently used temperature data and their limitations\nDaily\_air temperature\
  \ measurements are not available everywhere on Earth. The spatial coverage of temperature\
  \ measurements in Europe and North America is relatively good, but this is not always\
  \ the case for other continents, the oceans and the poles. If temperature is measured,\
  \ the data aren't always freely available and/or the time series sometimes contain\
  \ gaps or have a limited length."
layout: base_eustace
order: 0
permalink: /users/why-a-new-temperature-dataset/
title: Why a new temperature dataset?
---

<h2><strong>Currently used temperature data and their limitations</strong><img alt="Source: G. Lenderink" height="312" src="{{ site.baseurl }}/assets/media/uploads/temperatuur.jpg" style="float: right;" width="500"><a href="http://eustace-project.ceda.ac.uk/eustace/static/media/uploads/temperatuur.jpg"></a></h2>
<p>Daily air <strong>temperature measurements are not available everywhere</strong> on Earth. The spatial coverage of temperature measurements in Europe and North America is relatively good, but this is not always the case for other continents, the oceans and the poles. If temperature is measured, the <strong>data aren't always freely available</strong> and/or the<strong> time series sometimes contain gaps or have a limited length</strong>.</p>
<p>People interested in a specific location often use data collected at meteorological stations. Those working on larger regions often use one of the global datasets mentioned in the <em><a href="https://climatedataguide.ucar.edu/climate-data/global-temperature-data-sets-overview-comparison-table">Climate Data Guide</a> </em>or for Europe the <em><a href="http://www.ecad.eu/download/ensembles/ensembles.php">E-OBS</a> </em>dataset. Also <em><a href="https://climatedataguide.ucar.edu/climate-data/atmospheric-reanalysis-overview-comparison-tables">re-analysis data</a> </em>are used. However, the<strong> spatial resolution</strong> of these large datasets is <strong>often limited</strong> (often &gt;0.5 degree , which means that the data are given for grid boxes of about 50*50 km), or the temporal resolution is limited (regularly no daily data, but monthly averages are given).</p>
<p></p>
<p></p>
<h3><strong>Which of these limitation can be solved and how? </strong></h3>
<p>Satellite data can be used to <strong>estimate temperatures at locations where no ground or in situ observations are available</strong>. They have a relatively <strong>high spatail resolution and daily data</strong> can be provided. Satellites, however, measure skin temperature (the temperature at the surface; see figure below) and not air temperatures as are measured at meteorological station (standard at about 2 m height, this is relatively near the surface and therefore also called "surface air temperature"). The surface skin temperature of roofs or bare soil may differ considerably from the air temperature on a sunny day, but at other moments the skin and air temperatures may be more or less the same.</p>
<p><img height="258" src="{{ site.baseurl }}/assets/media/uploads/skin_air_temperature.jpg" width="600"></p>
<p>Therefore, to profit from available satellite data, the relationships between traditional (land and marine) surface air temperature measurements and satellite measurements (i.e. Land Surface Temperature, Ice Surface Temperature, Sea Surface Temperature and Lake Surface Water Temperature) have to be understood. These relationships have been derived empirically or with the help of physical models.</p>
<p>In the era before the satellite measurements the above approach cannot be used. However, with <strong>statistical techniques the spatial relationships between temperatures at different locations can be determined</strong> and these relationships can be used <strong>to extrapolate temperatures back in time</strong> for all locations on earth. Satellites can not measure the temperature of the surface of the earth on locations with clouds. The same statistical techniques can be used to fill the gaps in the era with satellite data.</p>
<p>The EUSTACE datasets <strong>are made freely available</strong>.</p>
<p></p>
<h3> <b>EUSTACE: differences from other surface temperature data sets</b></h3>
<ul>
<li>Globally complete daily dataset from 1850 on;</li>
<li>Designed in collaboration with users;</li>
<li>Validated information on the certainty of each daily value as an integral component;</li>
<li>Air temperature over the ocean, rather than sea surface temperature;</li>
<li>Use information from satellites to estimate air temperature over all surfaces of Earth;</li>
<li>New statistical techniques to create complete pictures of air temperature everywhere.</li>
</ul>
