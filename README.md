# FOSE 1025 Scientific Computing Exercises
The following exercises illustrate the kinds of questions that would be asked in parts of the unit and in the final project at FOSE1025, Macquarie University. Each question in this document uses different data. In the final project, ideally all questions would be based on a scenario and associated data.

The exercises have been designed with the Excel tool in mind. Feel free to suggest alternative or additional questions of the same kind which might be more suitable for MATLAB.

## 1. Import data
1. The idea of this exercise would be to read CSV tables, but some of the CSV would not have commas as separators.
2. Another exercise would read multiple CSV files and combine them into one table, for example by using Excel's VLOOKUP. This link shows an example of such an exercise: https://www.wiseowl.co.uk/excel/exercises/standard/lookup-functions/2233/


## 2. Data cleaning

The following course demonstrates various aspects of data cleaning using Excel.

https://www.linkedin.com/learning/excel-2016-cleaning-up-your-data/

Replicate the following tasks:

1. Eliminate empty rows and columns: https://www.linkedin.com/learning/excel-2016-cleaning-up-your-data/use-sort-to-eliminate-empty-rows-and-columns
2. Remove leading single quotes: https://www.linkedin.com/learning/excel-2016-cleaning-up-your-data/remove-leading-single-quotes
3. Split unusual date formats into columns: https://www.linkedin.com/learning/excel-2016-cleaning-up-your-data/split-unusual-date-formats-into-columns
4. Use Flash Fill for faster combining and splitting: https://www.linkedin.com/learning/excel-2016-cleaning-up-your-data/use-flash-fill-for-faster-combining-and-splitting
5. Adjust phone numbers and SS numbers for consistency: https://www.linkedin.com/learning/excel-2016-cleaning-up-your-data/adjust-phone-numbers-and-ss-numbers-for-consistency
6. Remove duplicate rows: https://www.linkedin.com/learning/excel-2016-cleaning-up-your-data/remove-duplicate-rows-from-a-list
7. Correct misspellings: https://www.linkedin.com/learning/excel-2016-cleaning-up-your-data/correct-multiple-misspellings


The following spreadsheet contains data that has been input manually and by different people, and consequently it has errors. Fix the errors. This is a small spreadsheet and the errors can be fixed one by one by re-typing the cells. But assume that there are many more rows and you cannot just edit the cells one by one. What would you do?

https://docs.google.com/spreadsheets/d/12NoKe86tCH3OZTeqxRNCwRQ5u1ygbfXwXYnqgC6gfwo/edit#gid=420693080

Below is a description of the data set from https://makingnoiseandhearingthings.com/2018/04/19/datasets-for-data-cleaning-practice/

    Couple of messy but easy data sets: NYC parents reporting their kids’ scores 
    on the gifted and talented exam, as well as school priority ranking. Some 
    enter the percentiles as point scores, some skip all together, no standard 
    preference format, etc. Also birth quarter affects percentiles.

## 3. Data transformation

This set of exercises would focus on removing columns that are not useful for subsequent data analysis, and creating new data columns with data that may be useful for subsequent analysis.

## 4. Scenario (Advanced): Weather data

The following link points to a data set of weather recordings in a region of Brazil. 

https://www.kaggle.com/PROPPG-PPG/hourly-weather-surface-brazil-southeast-region

However, the data needs to be cleaned and normalised in several ways. For example, this Kaggle kernel uses Python to clean the data and do some exploratory analysis. Try do to the same. 

https://www.kaggle.com/sanjayroberts1/exploratory-data-analysis-and-clean-up

Below is a quick description of the data and issues related to it, from https://makingnoiseandhearingthings.com/2018/04/19/datasets-for-data-cleaning-practice/ (typos not fixed)

    It’s covers hourly weather data from 122 weathers stations of southeast
    region (Brazil). The southeast include the states of Rio de Janeiro, São 
    Paulo, Minas Gerais e Espirito Santo. Dataset Source: INMET (National 
    Meteorological Institute – Brazil).

    Issues: Can you predict the amount of rain? Temperature? NOTE: Not all 
    weather stations started operating since 2000

Many of the tasks described here are probably too advanced for a first-year unit, and they would not be doable with Excel anyway. But if MATLAB can do them reasonably easily and without requiring a background in programming we might incorporate the tasks in the curriculum of the unit.


## 5. Scenario: Temperature sensors

The following CSV files contain artificially generated data and simulates the output of several temperature sensors, one sensor per file. Each CSV file includes a column with the time of the measure, and another with the value. The data, however, has several inconsistencies.

1. Several manufacturers serve different sensors, and consequently the column names are not identical. We know that one column represents the date, and the other represents the temperature. Device a method that identifies which is which.
2. Some sensors return the output in Celsius degrees, others return the output in Fahrenheit degrees. The final data set must have all data expressed in Celsius degrees.
3. The date format varies among manufacturers. When reading the data, normalise the dates to a uniform format.
4. Some sensors may have malfunctioned in some periods and consequently some measures may be missing. In addition, there may be multiple sensors from multiple manufacturers in the same place. The final data set will produce one column from each distinct region. If multiple sensors measure the same place, the data set must combine their measures in order to minimise missing data.
5. In the process to detect which sensors are in the same place, note that two sensors may use different temperature metric, and may have missing data at different times, and may occasionally produce a different measure (because of defects in the sensor).
