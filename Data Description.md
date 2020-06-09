## About Data

To tackle this problem, we need COVID-19 data for USA. The data should have Key Performance Metrics like number of cases, number of deaths, total population, state name, county name and most importantly this data should be at daily level (for each day). 

To get this data we will leverage, https://covidtracking.com/data/us-daily . This organization has developed COVID-19 data set for USA. They have created APIs that we can include in our codes or download a CSV file. For this analysis I have downloaded CSV file. It contains data from January to May. The dataset has following fields: 
**Field Name** | **Comment**
-----------|------------  
date | date
county | name of county
state | name of state
fips | Federal unique number, it is like zipcode
state_fips | Federal unique number for state
county_fips | Federal unique number for county
cases | number of positive cases
deaths | number of deaths
new_day_cases | number of new cases on that day
new_day_deaths | number of new deaths on that day
cases_per_capita_100k | number of cases per 100k population
deaths_per_capita_100k | number of deaths per 100k population
new_day_cases_per_capita_100k | number of new cases per 100k population
new_day_deaths_per_capita_100k | number of new deaths per 100k population
county_pop_2019_est | estimated population of county
pop_per_sq_mile_2010 | population per square mile as of 2010


Another requirement would be to get demographic values for these counties. I have download from Kaggle. CSV file contains following fields : 
**Field Name** | **Comment**
-----------|------------  
state_fips | Federal unique number for state
county_fips | Federal unique number for county
county | name of county
tot_pop | total population of that county
male_perc | % of Male population of that county
female_perc | % of Female population of that county
Age_0to4 | Number of population between age range 0-4
Age_5to14 | Number of population between age range 5-14
Age_15to24 | Number of population between age range 15-24
Age_25to34 | Number of population between age range 25-34
Age_35to44 | Number of population between age range 35-44
Age_45to54 | Number of population between age range 45-54
Age_55to64 | Number of population between age range 55-64
Age_65to74 | Number of population between age range 65-74
Age_75to84 | Number of population between age range 65-84
Age_84Plus | Number of population between age > 84

Last but not the least we will use FourSquare API to explore these counties and recommend outdoor activities and places for people to go out. https://developer.foursquare.com/docs/venues/explore
