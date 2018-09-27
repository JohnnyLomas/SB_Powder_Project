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


#### Importing and Cleaning the Data

- Data downloaded as fixed with ASCII
- Converted to CSV in excel
- Data read into pandas using pandas.read_csv()
- Missing data converted to NaN
- Numeric data converted from string to float
- Column added containing month as string
- Column added containing change in snow depth
- Column data types converted from object to numeric
- Months with missing data stored in a dictionary as year-month pairs


#### Summary Statistics

- Whole dataframe summarized using describe() function from pandas
- Daily average precipitation computed by month with variance 
- Compute the average total precipitation by month excluding months with missing data
