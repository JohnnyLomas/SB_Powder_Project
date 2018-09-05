## Sugar Bowl Powder Inference: Documentation

### Motivation

The goal of this project practice concepts and techniques related to exploratory data analysis
and statistical inference. This project is motivated by my desire to is to use daily weather data from the [remote weather station](https://raws.dri.edu/cgi-bin/rawMAIN.pl?caSUGB)
at Sugar Bowl Ski Resort to infer precipitation events at the resort. The project will 
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

The weather station was located using the [Tahoe Climate Information Management System](https://tahoeclim.dri.edu/). 
The dataset was obtained from the weather station's [webpage](https://raws.dri.edu/cgi-bin/rawMAIN.pl?caSUGB). The complete original dataset contains daily 
weather summary information related to precipitation, temperature, humidity, solar radiation, barometric pressure and windspeed. It covers
the period from Octobet 1st 2008 to October 31st 2016. The dataset is available on my GitHub page [here](www.snowbrains.com). Note that
the weather station was not operational for certain lengths of time during the study period and that data is missing for these peroids.

### Importing the Data

The data downloaded in ASCII text format from the weather station's database and formatted as a csv in Microsoft Excel.

