# US Accidents Exploratory Data Analysis

This project performs an exploratory data analysis (EDA) on a dataset of US accidents. The goal is to uncover insights and patterns in the data that could be useful for preventing future accidents and understanding the factors that contribute to them.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Data Preparation and Cleaning](#data-preparation-and-cleaning)
- [Exploratory Analysis and Visualization](#exploratory-analysis-and-visualization)
- [Ask and Answer Questions](#ask-and-answer-questions)
- [Summary and Conclusions](#summary-and-conclusions)
- [Requirements](#requirements)
- [How to Run](#how-to-run)

## Introduction

This project analyzes a dataset of US accidents to extract meaningful insights and patterns. The analysis covers various aspects of accidents, such as their frequency by city, time, weather conditions, and more. This information can be valuable for policymakers, city planners, and the general public to understand and mitigate accident risks.

## Dataset

The dataset used for this analysis is sourced from [Kaggle](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents). It contains information about accidents in the US, excluding data from New York. The dataset includes the following columns:

- ID
- Source
- Severity
- Start_Time
- End_Time
- Start_Lat
- Start_Lng
- End_Lat
- End_Lng
- Distance(mi)
- Description
- Street
- City
- County
- State
- Zipcode
- Country
- Timezone
- Airport_Code
- Weather_Timestamp
- Temperature(F)
- Wind_Chill(F)
- Humidity(%)
- Pressure(in)
- Visibility(mi)
- Wind_Direction
- Wind_Speed(mph)
- Precipitation(in)
- Weather_Condition
- Amenity
- Bump
- Crossing
- Give_Way
- Junction
- No_Exit
- Railway
- Roundabout
- Station
- Stop
- Traffic_Calming
- Traffic_Signal
- Turning_Loop
- Sunrise_Sunset
- Civil_Twilight
- Nautical_Twilight
- Astronomical_Twilight

## Data Preparation and Cleaning

The dataset is loaded using Pandas and cleaned to handle missing or incorrect values. Here are the steps taken for data preparation:

1. **Load the data in chunks** to handle memory efficiently.
2. **Concatenate all chunks into a single DataFrame**.
3. **Inspect the data** for missing values and incorrect data types.
4. **Fix missing values** by analyzing the percentage of missing data per column.

## Exploratory Analysis and Visualization

The exploratory analysis involves visualizing various aspects of the data to uncover insights. The following analyses were performed:

1. **City-wise accident analysis**:
   - Distribution of accidents across cities.
   - Top 20 cities with the highest number of accidents.

2. **Time-wise accident analysis**:
   - Distribution of accidents by hour of the day.
   - Distribution of accidents by day of the week.
   - Comparison of weekday and weekend accident patterns.
   - Monthly and yearly trends in accidents.

3. **Geospatial analysis**:
   - Scatter plot of accidents by latitude and longitude.
   - Heatmap visualization of accident locations using Folium.

## Ask and Answer Questions

Here are some key questions addressed in this analysis:

1. **Are there more accidents in warmer or colder areas?**
2. **Which 5 states have the highest number of accidents? How about per capita?**
3. **Does New York show up in the data? If yes, why is the count lower if this is the most populated city?**
4. **Among the top 100 cities in number of accidents, which states do they belong to most frequently?**
5. **What time of the day are accidents most frequent in?**
6. **Which days of the week have the most accidents?**
7. **Which months have the most accidents?**
8. **What is the trend of accidents year over year (decreasing/increasing)?**
9. **When is accidents per unit of traffic the highest?**

## Summary and Conclusions

Key insights from the analysis:

- No data from New York is present in the dataset.
- The number of accidents per city decreases exponentially.
- Less than 8% of cities have more than 1000 yearly accidents.
- Over 1000 cities have reported just one accident, indicating potential data quality issues.

## Requirements

To run the analysis, the following Python libraries are required:

- Pandas
- NumPy
- Seaborn
- Matplotlib
- Folium
- OpenDatasets
- Jovian

Install the required libraries using the following command:

```bash
pip install pandas numpy seaborn matplotlib folium opendatasets jovian
