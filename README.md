# AVIATION EVALUATION STRATEGY PROJECT

## Project Overview 

The aim of the project is to assist stakeholders in evaluating the risks associated with various aircraft models, thereby guiding informed purchasing decisions for commercial and private enterprises as part of the company’s diversification strategy into the aviation industry.As the stakeholder seeks to expand its portfolio into the aviation sector.


## Business Problem

Your company is expanding in to new industries to diversify its portfolio. Specifically, they are interested in purchasing and operating airplanes for commercial and private enterprises, but do not know anything about the potential risks of aircraft. You are charged with determining which aircraft are the lowest risk for the company to start this new business endeavor. You must then translate your findings into actionable insights that the head of the new aviation division can use to help decide which aircraft to purchase.

## Business understanding

Understanding the aviation industry landscape is essential for stakeholders as they explore diversification. This involves recognizing market dynamics, Aircraft models, and risks associated with the aviation industry.

We must fufil the following to provide reccomandations to the stake holders:
-Stake holders goals
-Risk aversion(accidents,fatalities,injuries...etc)
-Financial considerations



##  Data Understanding & Data  Analysis

### Data source 
this is the data sorce to be used in this analysis project [dataset](https://www.kaggle.com/datasets/khsamaha/aviation-accident-database-synopses)from the National Transportation Safety Board that includes aviation accident data from 1962 to 2023 about civil aviation accidents and selected incidents in the United States and international waters. 

### Data understanding
-Firstly we convert our csv file into a dataframe, so it easier to clean and analysis(overall better to work with sorted data)
-***Data understanding involves gathering and exploring relevant data*** to gain insights into the aviation industry and aircraft models.
-Key aspects include **assessing data quality, completeness, and relevance, as well as understanding the variables.**


### Data cleaning
-After understanding the kind of data we have access to we must clean it
-Data cleaning is a critical process that involves **identifying and rectifying inaccuracies, inconsistencies, and missing values within the collected datasets.**
- We identified the percentage(%) of total number of values missing in all columns.This provides a basis on each column and their relevance to provide key insights to our project.
- Columns missing a higher % of data are dropped and columns not required in our analysis are dropped eg. Latitude,Longitude,Schedule...etc
-We the remove duplicates, standarde formats, filling in missing information through estimation

![image](https://github.com/user-attachments/assets/2d4b4acf-6142-4c2b-8fda-6e4b94a49c62)



### Data Aggregation
-After cleaning and preparing our data now we must group the data to find insights.
-Data aggregation involves **compiling and summarizing raw data to create a cohesive dataset that highlights key trends and insights**.
-We use the **.groupby()** method on various columns in our data eg. Model & Total.Fatal.Injuries, Make & Total.Fatal.Injuries...etc
-This process typically includes grouping data by specific attributes, such as Model,Country, Injury.Severity ,Country,Aircraft.damage,Aircraft.Category...etc


### Data visualisation
-This is the last step, we must create **graphical represantions of our data.So it can be undestood and interpreted better.**
-Make  + Total.FAtal.Injuries **piechart**, show the top 10  makes with the most fatal inuries .
-**line graph** between Total.FAtal.Injuries aand year, shows us the tiemframe in which these  fatalitie ha ppened  



### Recomendations
following analysis and everyother step above the following would be my recommendations:
-**Prioritize purchase of newer aircrafts**- the linegrph showed us us time went on the newer planes were less likely to get in accidents based of on the data
-**Consider routes with better weather condituions**  -  the boxplot shows us that the weather was a cosiderable factor when considering the likely-hood of an accident, better weather would be something to consider in terms of the aircrafts route
-**public sector would be a better investment than private sector**- planes used for the purpose of private usage were more likely to crash.

### Conclusion
through this analysis project we identified clear pattern recognition for our stakeholders to consider as they look to expand into the aviation indusrty
For a better and deeper understabnding of the visualisation can be accesed on the tableau linnk:
https://public.tableau.com/app/profile/imran.awadh/viz/phase1tableau/Dashboard1?publish=yes





   
