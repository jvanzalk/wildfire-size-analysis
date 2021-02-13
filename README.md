# wildfire-deep-learning

The goal of this project was to create a model to predict the sizes of wildfires in British Columbia, Canada. 

Wildfire records were scraped from this BC government webpage: https://www2.gov.bc.ca/gov/content/safety/wildfire-status/about-bcws/wildfire-statistics

Exploratory analysis and feature engineering was performed. This plot of wildfires was produced to examine geographical trends in wildfire size:



After cleaning up the data, two models were compared: a simple multi linear regression and a regression with Tensorflow. While the Tensorflow model performance was the better, both models lacked any real predictive ability.

The features (month, year, latitude, longitude) explained less than 10% of variance in fire sizes. In this case, additional features are needed to improve the results. 

Recommended actions: 
- Replace month with weather data
- Humans cause the majority of wildfires so look at travel data (e.g., Airbnb) or population.
