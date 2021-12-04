# wildfire-size-analysis

The goal of this project is to create a model to predict the sizes of wildfires in British Columbia, Canada. 

Wildfire records were scraped from this BC government webpage: https://www2.gov.bc.ca/gov/content/safety/wildfire-status/about-bcws/wildfire-statistics

Exploratory analysis and feature engineering was performed on the scraped data. This plot of wildfires was produced to examine geographical trends in wildfire size:

![](https://github.com/jvanzalk/wildfire-deep-learning/blob/main/Images/hotspots.png)

In addition to the features aquired from the scraped data (season, year, latitude, longitude), more features were added using spatial operations from geopandas.

Given that Humans cause the majority of wildfires, the minimum distance of fires to major roads was calculated to determine proximity of fires to human populations. 

Granular weather data was not available so a spatial join was performed to determine what biogeoclimatic zone each fire was located in. These zones are classifications based on types of vegitation, soil, and other factors.

The next step is to create a model to understand how these features affect wildfires sizes and make predictions.
