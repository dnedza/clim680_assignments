## Exploring Global Relationships Between Surface Temperature and North Atlantic Variability 
 
## Douglas Nedza

## Introduction

For CLIM 680, I will be investigating the relationship between North Atlantic Temperature Variability measured between 80W-0W and 0N-60N, and other surface variables, such as sea surface temperature (SST), surface temperature (TS), and precipitation (PRECT) across the globe.

North Atlantic Variability is well studied, with demonstrated importance for predictability and regional climate.  Changes in surface temperature in the North Atlantic region may also be useful to monitor changes in the Atlantic Meridional Overturning Circulation, which bears great impact on Northern Hemisphere weather, and may be sensitive to anthropogenic forcing.

## Data

The data used in the following analyses are taken from the CMIP5 archive and currently include the NASA GISS E2 H model and the NOAA GFDL model (depending on script, as changes have been made in the dataset used in different scripts (to be changed)).

The data used is taken from pre-industrial runs, using constant external forcing replicating the year 1850.  The use of pre-indusitral model runs prevents results from demonstrating the dominance of the anthropogenic/volanic trends, as the desired relationships characterize the internal variability of the climate system.

__NOAA GFDL CM3__
[NOAA GFDL-CM3](https://www.gfdl.noaa.gov)

__NASA GISS E2-H__
[NASA GISS-E2-H](https://www.giss.nasa.gov)

## Analyses of Data

### General Characteristics of Data

To gain an appreciation of the general characteristics of the model output, who notebooks have been prepared for each model.  The first notebook assesses aspects of the mean and climatology for the sea surface temperature.  The second calculates principal components of the surface (2m) temperature.  These principal components characterize spatial and temporal patterns of variability that are orthogonal.

There does appear to be some differences in the SST climatologies between the models, with GISS-E2-H having warmer tropical regions, and GFDL-CM3 a warmer region near Scandanavia.  GFDL is also missing data in some regions of the Artic.

A difference between surface temerature and sea surface temperature is calculated.  Consistent between models, the SST tends to be slightly higher than the overlying atmospheric temperature.  This is exaggerated in high latitudes, where ice is formed and prevents the water from continuing to cool.

Evaluating the variability of surface temperature in each model reveals regions of large variability along the coast of Antarctica and north of Scandanavia.  The variability in these regions is more pronounced in GFDL-CM3, particularly over the Wendell Sea.  In GFDL-CM3 this variability near Antarctica dominates the first two princiapl components.

When restricting the domain to the North Atlantic, most of the variability is concentrated near the coast north of the Gulf Stream departure, with associted changes in temperature near the coast of Europe and Africa.  This is likely related to changes in subpolar SST and subsequent atmospheric changes.


[Visualize Mean and Climatological Characteristics of Sea Surface Temperature inGFDL-CM3](https://github.com/dnedza/clim680_assignments/blob/master/clim680_project_anoms_dnedza_NOAA.ipynb)

[Visualize Spatial Patterns of Surface Temperature Variability in GFDL-CM3](https://github.com/dnedza/clim680_assignments/blob/master/clim680_project_EOF_dnedza_NOAA.ipynb)

[Visualize Mean and Climatological Characteristics of Sea Surface Temperature in GISS-E2-H](https://github.com/dnedza/clim680_assignments/blob/master/clim680_project_anoms_dnedza_NASA.ipynb)

[Visualize Spatial Patterns of Surface Temperature Variability in GISS-E2-H](https://github.com/dnedza/clim680_assignments/blob/master/clim680_project_EOF_dnedza_NASA.ipynb)

### Teleconnections

Teleconnections are visualized by calculating composites, which can capture non-linear relationships in teleconnections, correlation, which measures the linear relationship between two time series, and quantifies this relationship on a scale between 0 and 1.  Linear regressions are also calculated, which quantify linear relationships, but do not have a predefined scale for the returned values. 

#### Atlantic Basin Average

[Visualize Spatial Patterns of Teleconnections Associated with Atlantic Variability in GFDL-CM3](https://github.com/dnedza/clim680_assignments/blob/master/clim680_project_amv_dnedza_NOAA.ipynb)

[Visualize Spatial Patterns of Teleconnections Associated with Atlantic Variability in GISS-E2-H](https://github.com/dnedza/clim680_assignments/blob/master/clim680_project_amv_dnedza_NASA.ipynb)


#### ENSO

Comparing the NINO3.4 indices calculated for each model, it is apparent that GFDL-CM3 exhibits variability in this region of greater amplitude than GISS-E2-H.  This could be a consequence of sub-annual behavior in this region, as this index is calculated as an annual mean.  This is not the most appropriate timescale for this index due to shorter (2-3 years) time scale that typically characterizes ENSO variability as well as the tendency of ENSO to change within a single year.A better use of annual mean could be calculated from July-June.

There does not appear to be much non-linear relationships in this data, therefore, each method of calculating the teleconnections reveals similar information.  Changes in the index has limited impacts in global SST.  While surface temperature changes are more widespread globally, affecting regions over landmasses, the region of significance are generally confined to the central Pacific.  Precipiation changes are also confined to the central Pacific region.  GFDL-CM3 tends to have larger regions of significant impacts globally.

When restricting the analysis to the North Atlantic, a statistically significant relationship is found in the tropical region, with a larger region of significance found in GFDL-CM3.  This relationship is of the same sign, whereby a warm ENSO anomaly is associated with a warming of the tropical Atlantic.  GISS-E2-H also has a small region of significance of the opposite sign over the central Atlantic.

[Visualize Spatial Patterns of Teleconnections Associated with ENSO in GFDL-CM3](https://github.com/dnedza/clim680_assignments/blob/master/clim680_project_nino_dnedza_NOAA.ipynb)

[Visualize Spatial Patterns of Teleconnections Associated with ENSO in GISS-E2-H](https://github.com/dnedza/clim680_assignments/blob/master/clim680_project_nino_dnedza_NASA.ipynb)

### Conda Environment
A environment.yml file is available to define a consistent environment for the execution of the above codes.

## Summary

 
