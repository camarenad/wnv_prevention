# README.md

## Authors
Daniel Camarena | https://github.com/camarenad. 
Jon Johnson | https://github.com/jonjohnsontc. 
Carl Lehman | https://github.com/celehman44. 

Our consulting team, #VanessaCarlton, Inc (VCI) has been on the frontlines of virology and epidemiology research for years. Our group is responsible for key discoveries in viral transmission, most notably of which, our 2002 paper on superviruses falling 'into' the sky.

We've been contracted by the Centers for Disease Control (CDC) to report on the prevelance of West Nile Virus (WNV) in the Chicago area, and effective means of control. For this study, we reviewed a number of datasets on mosquito captures, mosquito pesticide sprays, and weather conditions in Chicago, ranging from 2007 to 2014, provided by the city of Chicago on Kaggle servers, the trusted administrator of government information. Given this, we decided to focus our study on mosquito populations and their transmission of WNV to humans.

In order to conduct a thorough report, our team developed a machine learning model to predict the prevalence of WNV given a date, mosquito trap, and location in the Chicago area. Within the notebooks incldued, you'll find an extensive overview of the processes used to develop the model, and our  

We'd like to share that report with you here.

## Problem Statement: 
> How do certain weather events affect the presence of West Nile virus in the Chicago area? Can this problem effectively be tackled with Machine Learning?

## Executive Summary of Findings: 

Through our research, we've discovered a number of weather related conditions that do effect the growth of mosquitos, and thereby the presence of WNV:

- Out of all weather conditions, the level of moisture in the air provides the greatest influence on mosquito abundance.
- The combination of "optimal" mosquito weather conditions are what cause the largest gain in the presence of WNV.

The most important weather related condition turned out to be Wet Bulb temperatue, which again makes a lot of "common" sense. The higher the Wet Bulb temperature, the more relative humidity. Of course, the more relative humidity, the greater the saturation of water in the air, and the greater potential for mosquitos (and WNV) to spread.

The remaining weather related conditions are all clustered with a similar importance. This shows us that while each feature has an effect on the prediction, no-single one of them could provide enough influence to shift a prediction of WNV from negative to positive. We see this as confirming that it's the sum of all mosquito-optimal weather conditions in concert that allow mosquitos to proliferate (and potentially spread disease).

You can find additional information within the included jupyter notebooks.

## Organization

This project is divided into five different folders, which we've provided a rundown of here:

- `assets` - contains python variables used in the modeling process
- `data`: all of the datasets we received from the City of Chicago, along with several permutations of the datasets that we created to get a better grasp of the data.
  - Mosquito trap data from 2007 to 2014
  - Weather data from 2007 to 2014 from the [NOAA](http://cdo.ncdc.noaa.gov/qclcd/QCLCD?prior=N)
  - GIS pesticide spraying locations from 2011 and 2013
- `images`: contains images generated within my notebooks and utilized in the presentation file
- `notebooks`: - contains the actual project documents
  - `01_Cleaning.ipynb`: Ensuring that our data sources are clean, and that they're ready for EDA as a combined dataset, along with feature engineering.
  - `02_EDA.ipynb`: Conducting exploratory data analysis ("EDA") on our combined dataset, plotting a number of weather-related features against mosquito abundance in order to get a better idea of the most important features, and transforming our data through feature engineering to ready it for preprocessing and model fitting.
  - `03_Preprocessing`: Processing our carefully engineered data to utilize for modeling
  - `04_Random_forest_model.ipynb`: Building our random forest model, and testing it on the data provided to us.
  - `4a_log_reg_model.ipynb`: Building our logisitc regrssion model, and testing it on the data provided to us.
  - `i_Cleaning_spray.ipynb`: Cleaning the spray data provided. This data is not used beyond this notebook, however
  - `ii_EDA_lag_search.ipynb`: Looking over each of the weather related features. These weather features are also manipulated to determine how they interact with mosquito abundance.
  - `iii_Submission.ipynb`: In order to test the effectiveness of our model, it was submitted to a Kaggle competition on detecting WNV in mosquitos. This notebook contains the setup of our submission.
- `presention`: PDF slides of a presentation that we made on 9/28/2018
