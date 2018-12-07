# SB_Powder_Poject

### Jump-To

[Motivation](#motivation)

[Code](#code)

[Reports](#reports)

[Data Set](#data-set)

[Driving Questions/Hypotheses](#driving-questions/hypotheses)

[Conclusions](#conclusions)

### Motivation

The goal of this project is to practice concepts and techniques related to exploratory data analysis
and modeling natural phenomena. During the project I will use daily weather data from the [remote weather station](https://raws.dri.edu/cgi-bin/rawMAIN.pl?caSUGB)
at Sugar Bowl Ski Resort to observe weather trends leading to precipitation and to predict future 
precipitation events. The analysis was performed using both python and R.

### Code 

The code for this project is provided in a set of ipython notebooks and Rmarkdown documents. Links to these files
are provided below:

- Data cleaning and summary statistics: [Ipython Notebook](https://github.com/JohnnyLomas/SB_Powder_Project/blob/master/ExploratoryAnalysis.ipynb)
- Distributions and scatter plots: [Rmarkdown](https://github.com/JohnnyLomas/SB_Powder_Project/blob/master/Distributions.Rmd)
- Regression Modeling: [Rmarkdown](https://github.com/JohnnyLomas/SB_Powder_Project/blob/master/Modeling.Rmd) 
- PCoA and PCoR: [Rmarkdown](https://github.com/JohnnyLomas/SB_Powder_Project/blob/master/PCoA.Rmd)

### Reports

The knitted Rmarkdown documents are provided in both PDF and HTML format. The PDFs are easily viewable in Github, but do not include Plotly HTML widgets. The HTMLs can be downloaded and viewed seperately. 

- Distributions and scatter plots: [PDF](https://github.com/JohnnyLomas/SB_Powder_Project/blob/master/Distributions.pdf), [HTML](https://github.com/JohnnyLomas/SB_Powder_Project/blob/master/Distributions.html)
- Regression Modeling: [PDF](https://github.com/JohnnyLomas/SB_Powder_Project/blob/master/Modeling.pdf), [HTML](https://github.com/JohnnyLomas/SB_Powder_Project/blob/master/Modeling.html)
- PCoA and PCoR: [PDF](https://github.com/JohnnyLomas/SB_Powder_Project/blob/master/PCoA.pdf), [HTML](https://github.com/JohnnyLomas/SB_Powder_Project/blob/master/PCoA.html)

### Data Set

The weather station was located using the [Tahoe Climate Information Management System](https://tahoeclim.dri.edu/). 
The dataset was obtained from the weather station's [webpage](https://raws.dri.edu/cgi-bin/rawMAIN.pl?caSUGB). The complete original dataset contains daily 
weather summary information related to precipitation, temperature, humidity, solar radiation, barometric pressure, snow depth, and windspeed. It covers
the period from December 1st 2005 to December 31st 2016. The dataset is available on my GitHub page [here](www.snowbrains.com). Note that
the weather station was not operational for certain lengths of time during the study period and that data is missing for these peroids.


Factor Units:
- Solar Radiation (kW-hr/m^2)
- Precipitation (mm) 
- Temperature (C)
- Humidity (%)
- Barometric Pressure (mbar)
- Windspeed (m/s)
- Snow Depth (mm)

### Driving Questions and Hypotheses

**Hypotheses**

1. Temperature, pressure, and relative humidity play a large role in precipitation events
2. March is typically the snowiest month at Sugar Bowl


**Questions**

1. What is the snowiest month at Sugar Bowl on average
2. What factors are most important for determining the occurence of precipitation events 
3. Can I effectively model multiple variable relationships to predict precipitation events using linear regression techniques?

### Conclusions 

Largely, the conclusioins of this analysis followed along the lines of intuition. For example, the distributional analysis indicated that precipitation events occur during low pressure, low temperature systems when there is low solar radiation and high humidity. Interestingly, according to principle component analysis, solar radiation represented the largest total portion of the variation in the data set. This makes sense intuitively because clouds must be present for precipitation to occur. Another interesting observation was that the largest precipitation events seem to occur when the daily average temperature is close to zero degrees celcius. December is the snowiest month on average at Sugar Bowl but with the highest variance; however, March is the next snowiest month with a much lower varaince. This may be why March is often thought of as the snowiest month in the Sierra; it's simply more consistent. 

All the models fitted to the weather data had low Adjusted R-squared values and thus, had low predictive abilities. The highest Adjusted R-squared reached for any model was approximately 0.4. This was likely due to the fact that days with similar pressure, temperature, radiation, and humidity had both low and high precipitation results. This problem also negatively effected the models by introducing heteroskedasticity and non-normality of the errors. Evidently, other factors are needed to effectively predict precipitation events. 
