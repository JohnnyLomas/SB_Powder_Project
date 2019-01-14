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

### Driving Hypotheses

1. Temperature, pressure, and relative humidity play a large role in precipitation events
2. March is typically the snowiest month at Sugar Bowl
3. Precipitation events can be effectively modeled using linear regression techniques


### Conclusions 

1. Temperature and humidity clearly played a large role in precipitation events at Sugar Bowl Ski Resort during the study peroid, but the effect of pressure was less well defined. Temperatures close to 0 degrees Celsius and high values of relative humidity (~90-100%) were the most favorable for precipitation events. Pressure readings associated with precipitation events were more variable and do not seem to be a good predictor of precipitation. Interestingly, solar radiation appeared to play a large role due to the fact that it was almost perfectly aligned with the first principle component in the principle component analysis. 
2. On Average, December was the snowiest month in the study period; however, this average was accompanied by the largest variance. March was the second snowiest month on average with much smaller variance relative to December. 
3. The predictive ability of all linear models fit to the dataset was low due to the fact that precipitation producing conditions of temperature, pressure, solar radiation, and humidity also produced days with no precipitation. More factors are needed to deconvolute precipitation producing days from non-producing days with the same condiitons. No model achieved an adjusted R-squared greater than ~0.4. Severe multicollinearity and heteroskedasticity problems were prevelant in the data and transformations such as Principle Component Analysis and Box-Cox Transformation were employed to alleviate these problems. The highest performing model was selected using fourth-degree polynomial terms. 

