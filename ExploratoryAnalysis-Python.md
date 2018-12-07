## Sugar Bowl Powder Project: Exploratory Data Analysis with Python



#### Jump To


[Hypotheses and Guiding Questions](#iypotheses-and-guiding-questions)
[Importing and Cleaning the Data](#importing-and-cleaning-the-data)
[Summary Statistics](#summary-statistics)

#### Hypotheses and Guiding Questions

This section summarizes the hypotheses and questions which guided this analysis:

**Hypotheses**

1. Temperature, pressure, and relative humidity play a large role in precipitation events
2. March is typically the snowiest month at Sugar Bowl


**Questions**

1. What is the snowiest month at Sugar Bowl on average
2. What factors are most important for determining the occurence of precipitation events 
3. Which were the largest snow years in the study period 
4. Which month had the largest total snowfall in the study period
5. What is the average yearly snowfall at Sugar Bowl
6. Can I effectively model the single, double, multiple variable relationships to predict precipitation events?


#### Importing and Cleaning the Data

- Data downloaded as fixed with ASCII
- Converted to CSV in excel
- Data read into pandas using pandas.read_csv()
- Missing data converted to NaN
- Numeric data converted from string to float
- Column added containing month as string
- Column added containing change in snow depth
- Column data types converted from object to numeric
- Months with missing data stored in a dictionary


#### Summary Statistics

- Whole dataframe summarized using describe() function from pandas
- Daily average precipitation computed by month with variance 
- Daily average and standard deviation computed for all relevant factors
- Compute the average total precipitation by month excluding months with missing data
- Plotted monthly average precipitation as a bar chart with error bars
- Plotted daily average values for each relevant variable by month
- Exported CSV's for use in R

#### Distributions

- Plot single variable distributions by probability density
- Plot single variable scatter plots to total precipitation
- Plot two-variable scatter plots with precipitation

#### Modeling 
- Principle component analysis (dimensionality reduction)
- Regression model with top few principal components
- Other model types with principal components
- Machine learning model
	
