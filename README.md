# Space Missions Data Exploration

## by Christabel Onwuka


## Introduction

This is my third project in the Udacity/ALX-T Data Analyst Nanodegree Program. The project, Communicate Data Findings, is focused on demonstrating the importance and value of data visualization (both exploratory and explanatory) techniques in the data analysis process choosing one's own dataset or a Udacity-curated dataset.


## Dataset

The dataset used, Space Missions Data, contains information on all the space missions in human history (from 1957 to August 2022) and was gotten from [Maven Analytics Data Playground.](https://www.mavenanalytics.io/data-playground)

The dataset contains a csv table with 4,631 records, one for each space mission. Each record contains 
details on each mission's name, location, date, and status of the launch, the company responsible, and 
the price, status, and name of the rocket.

The dataset was wrangled methodically and quality issues such missing values, erroneous datatypes and 
duplicated rows were cleaned. Also tidiness issues which included column splitting and creation of new 
columns were performed on the dataset before it was analyzed and visualized to find out the patterns and 
trends in mission status of space missions, rocket status and price over the years and across countries.


## Summary of Findings

In the exploration, I found that:

- There is a weak negative correlation between year and price of rockets 
because after the year 1990, a significant decline in the price of rockets till date is seen. From the 
late 2010's upwards, a high density of rockets with lower prices in use is observed.

- The distribution of the variable of interest, the `mission_status` shows that about 95% of all space
missions were successful; indicating a very high mission success rate with the number of active rockets 
twice the number of retired rockets. In this dataset, which the cleaned dataset with **no null values**, 
the USA is the country with the most launched space missions followed by China in second place and France
in the third place.

- In comparison with the original dataset which has some null price values, there seems to be a resurgence 
in space mission programs in recent years especially in the 2020's which show the highest space mission 
programs in human history.

- With an unusually high price for a rocket at 5 billion USD and the lowest price at 2.5 million dollars, 
most rocket prices lie below 500 million dollars. The rocket price range of active rockets lie below 500
million USD while the rockets with the outlier price range of between 1000 - 5000 million USD have all been retired. There is a very strong indication that cheaper or cost-effective rockets is the way forward in the
next wave of the space race.


## Key Insights for Presentation

For the presentation, I focus on the influence of price and year on the mission and rocket status of countries. I start by introducing the pattern in the distributions of the mission status and rocket status variables. Afterwards, I introduce the the relationship between the numeric variables, price and year, showing their correlation with a lineplot. 

Then, I look at the relationship of the categorical variables especially country and rocket status with the numerical variables of year and price. Since most missions were most likely to be successful, I omitted the relationship between the mission status with respect to both price and year as no useful insight was gained. 
I've made sure to vary the plots and color palettes for the presentation to make sure it is viewed from 
different perspectives using lineplots, barplots, and point plots.


## What I learned

After completing this project, I learned to:

- Supplement statistics with visualizations to build understanding of data.
- Choose appropriate plots, limits, transformations, and aesthetics to explore a dataset, allowing me to understand distributions of variables and relationships between features.
- Use design principles to create effective visualizations for communicating findings to an audience.


## Resources used

 - [pandas.Series.dt.year](https://pandas.pydata.org/docs/reference/api/pandas.Series.dt.year.html) to extract year from date values.
 
 - [Extracting year from pandas datetime](https://stackoverflow.com/questions/62021214/extract-year-from-pandas-datetime-column-as-numeric-value-with-nan-for-empty-cel).
 
 - [Re-ordering columns](https://stackoverflow.com/questions/53141240/pandas-how-to-swap-or-reorder-columns).

 - [Right splitting columns and adding element to new column](https://stackoverflow.com/questions/38498718/split-pandas-column-and-add-last-element-to-a-new-column).

 - [Replacing commas and converting to floats](https://stackoverflow.com/questions/65510896/converting-string-to-float-in-pandas).
 
 - [Combining date time and changing its datatype](https://stackoverflow.com/questions/17978092/combine-date-and-time-columns-using-python-pandas).
