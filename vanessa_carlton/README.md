# README.md

Our consulting team, #VanessaCarlton, Inc (VCI) has been on the frontlines of virology and epidemiology research for years. Our group is responsible for key discoveries in viral transmission, most notably of which, our 2002 paper on superviruses falling 'into' the sky.

We've been contracted by the Centers for Disease Control (CDC) to report on the prevelance of West Nile Virus (WNV) in the Chicago area, and effective means of control. For this study, we reviewed a number of datasets on mosquito captures, mosquito pesticide sprays, and weather conditions in Chicago, ranging from 2007 to 2014, provided by the city of Chicago on Kaggle servers, the trusted administrator of government information.

We'd like to share that report with you here.

## Problem Statement: 
> How do certain weather events affect the presence of West Nile virus in the Chicago area? Can this problem effectively be tackled with Machine Learning?

## Executive Summary of Findings: 

Given the extensive domain knowledge of Lebl, et al in the field, we generated features with the same shifted values as found in their paper, to see how our models performed. 

- Daytime Length averaged 4-5 weeks prior
- Temperature averaged 2 weeks prior
- Wind speed averaged over 3 weeks prior
- Daytime length may be the most important factor generating the seasonal pattern of mosquito abundance as it regulates - together with temperature

Wet-bulb -The lowest temperature that can be reached by evaporating water into the air. Note: the wet bulb temperature will always be less than or equal to the temperature. It feels more comfortable when wet-bulb temperature is low. This is a measure of the humidity in the air.  Humidity is a contributing factor to increased mosquito populations.

## Organization

This project is divided into four different folders, which we've provided a rundown of here:

- `data`: All represeting various elements of the city of Chicago 
  - Mosquito trap data from 2007 to 2014
  - Weather data from 2007 to 2014 from the [NOAA](http://cdo.ncdc.noaa.gov/qclcd/QCLCD?prior=N)
  - GIS pesticide spraying locations from 2011 and 2013
- `images`: contains images generated within my notebooks and utilized in the presentation file
- `notebooks`: - contains the actual project documents
  - `01_Cleaning.ipynb`: Ensuring that our data sources are clean, and that they're ready for EDA as a combined dataset, along with feature engineering.
  - `02_EDA.ipynb`: Conducting exploratory data analysis ("EDA") on our combined dataset, plotting a number of weather-related features against mosquito abundance in order to get a better idea of the most important features, and transforming our data through feature engineering to ready it for preprocessing and model fitting.
  - `03_Preprocessing`: Processing our carefully engineered data to utilize for modeling
  - `04_Random_forest_model.ipynb`: 
  - `4a_log_reg_model.ipynb`: 
  - `i_Cleaning_spray.ipynb`: Cleaning the spray data provided. This data is not used beyond this notebook, however
  - `ii_EDA_lag_search.ipynb`: Looking over each of the weather related features. These weather features are also manipulated to determine how they interact with mosquito abundance.
- `pickle` - contains python variables used in the modeling process

## Presentation

The presentation is designed to be referenced alongside the notebooks, and can be found at the following link: [HERE]()
