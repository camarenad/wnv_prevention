# README.md

Our consulting team, #VanessaCarlton, Inc (VCI) has been on the frontlines of virology, and epidemiology research for years. Our group is responsible for key discoveries in viral transmission, most notably of which, our 2002 paper on superviruses falling 'into' the sky.

We've been contracted by the Centers for Disease Control (CDC) to report on the prevelance of West Nile Virus (WNV) in the Chicago area, and effective means of control. For this study, we reviewed a number of datasets on mosquito populations in Chicago,   

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

This project is divided into four different folders:

- `data`: All represeting various elements of the city of Chicago 
  - Mosquito trap data from 2007 to 2014
  - Weather data from 2007 to 2014 from the[NOAA](http://cdo.ncdc.noaa.gov/qclcd/QCLCD?prior=N)
  - GIS pesticide spraying locations from 2011 and 2013
- `images`: contains images generated within my notebooks and utilized in the presentation file
- `notebooks`: - contains the actual project documents
  - `01_Cleaning.ipynb`: 
  - `02_EDA.ipynb`: 
  - `03_Preprocessing`: 
  - `04_Random_forest_model.ipynb`: 
  - `4a_log_reg_model.ipynb`:
  - `i_Cleaning_spray.ipynb`:
  - `ii_EDA_lag_search.ipynb`:
- `pickle` - contains python variables used in the modeling process

## Presentation

The presentation is designed to be referenced alongside the notebooks, and can be found at the following link: [HERE]()
