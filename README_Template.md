# <Repository Title>

<Instructions: copy and paste this template into your project README file (found in the parent folder of the repository). Fill in relevant information as requested.>

## Summary

The purpose of this repository is to explore if certain weather variables impact air quality in Stanislaus County, CA. Poor air quality is a significant concern in this region, often exacerbated by local environmental 
conditions and external influences such as wildfires and some industrial emissions. The primary focus is to identify patterns or correlations between weather conditions and changes in air quality metrics, such as PM2.5 concentrations. The goal of this project is to understand how specific weather variables, such as precipitation and temperature, impact air quality. This research will provide insights into 
seasonal and weather-related factors contributing to air pollution, offering a some insight for future mitigation strategies, public health advisories, or policy recommendations.


## Investigators

Ellie Harrigan
Lauren Ng
Rosalind Hu
Hanbing Lyu

## Keywords

air quality, stanislaus county, california, weather, noaa, PM2.5, pollution

## Database Information

This repository contains two key datasets:
1. EPA Air Quality Data: Downloaded from the EPA’s outdoor air quality database, this dataset includes daily AQI and PM2.5 readings for Stanislaus County.
2. Weather Data: From NOAA's weather. This dataset includes historical daily measurements of weather variables such as temperature.


## Folder structure, file formats, and naming conventions 

Folders included in the repository are "Data" "Raw" "Processed" and "Metadata" The raw data folder includes 10 raw datasets from the EPA air quality website. The processed folder will contain the finalized 
processed air and weather data. The metadata folder will contain the information on both the weather and air quality datasets. 

## Metadata

In the Stanislaus_Air_Processed dataset, there are eight columns: 
1) year_month: This displays the year-month from 2013-2023
2) avg_PM2.5: This has the average PM2.5 for each year/month from 2013-2023
3) max_PM2.5: This has the max PM2.5 for each year/month from 2013-2023
4) min_PM2.5: This has the min PM2.5 for each year/month from 2013-2023
5) total_records: Number of records for that year/month taken
6) month_year_date: This column reformatted the year_month column from a character to a date, it displays the date of year,month,day from 2013-2023
7) year: This columm just displays each year from 2013-2023
8) month: This column just displays each month from 2013-2023

In the Weather_Data_Processed dataset, there are six columns:
1) year_month: This displays the year-month from 2013-2023
2) avg_temperature: This has the average temperature for each year/month from 2013-2023 in Stanislaus County, CA
3) max_temperature: This has the max temperature for each year/month from 2013-2023 in Stanislaus County, CA
4) min_temperature: This has the min temperature for each year/month from 2013-2023 in Stanislaus County, CA
5) total_records: Number of records for that year/month taken
6) month_year_date: This column reformatted the year_month column from a character to a date, it displays the date of year,month,day from 2013-2023

<For each data file in the repository, describe the data contained in each column. Include the column name, a description of the information, the class of data, and any units associated with the data. Create a list or table for each data file.> 

Stanislaus_Air_Data_Processed
1) year_month: character
2) avg_PM2.5: number
3) max_PM2.5: number
4) min_PM2.5: number
5) total_records: integer
6) month_year_date: Date
7) year: character
8) month: character

Weather_Data_Processed
1) year_month: character
2) avg_temperature: number
3) max_temperature: number
4) min_temperature: number
5) total_records: integer
6) month_year_date: Date

## Scripts and code

openmeteo package was used to import the weather data from NOAA. 
