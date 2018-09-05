## Squaw Valley Powder Inference: Documentation

### Motivation

The goal of this project practice concepts and techniques related to exploratory data analysis
and statistical inference. This project is motivated by my desire to is to use daily weather data from the [remote weather station](https://www.ncdc.noaa.gov/cdo-web/datasets/GHCND/stations/GHCND:USS0020K30S/detail)
at Squaw Valley's High Camp to infer precipitation events at the ski resort. The project will 
progress according to the following steps:

	1. Finding an appropriate weather dataset
	2. Cleaning and importing the dataset
	3. Exploratory data analysis
		a. Observe single variable trends
		b. Explore multivariable trends
		c. Potting of distributions
	4. Generation of appropriate distributions for inference
	5. Construction of probability density functions and likelihood matrices
	6. Development of maximum likelihood prediction scheme
	
### Weather Data

The dataset was obtained from the National Oceanic and Atmospheric Administration (NOAA) using their
online [data tool](https://www.ncdc.noaa.gov/cdo-web/datatools/findstation). It contains daily 
weather summary information related to precipitation, temperature, humidity, and windspeed. It covers
the period from January 1st 2013 to January 1st 2017. The dataset is available on my GitHub page [here](www.snowbrains.com).

