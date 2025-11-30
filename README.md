# Weather Data Analysis Project

## Project Description

This project performs an exploratory data analysis on a weather dataset (`file.csv`). The analysis covers various aspects of the weather data, including wind speed, temperature, humidity, visibility, pressure, and weather conditions. The goal is to extract key insights and demonstrate common data manipulation and analysis techniques using the `pandas` library in Python.

## Dataset

The dataset used in this project is `file.csv`, which contains hourly weather data, including:
- `Date/Time`: Date and time of the observation
- `Temp_C`: Temperature in Celsius
- `Dew Point Temp_C`: Dew Point Temperature in Celsius
- `Rel Hum_%`: Relative Humidity percentage
- `Wind Speed_km/h`: Wind Speed in kilometers per hour
- `Visibility_km`: Visibility in kilometers
- `Press_kPa`: Pressure in kiloPascals
- `Weather`: Describes the weather condition (e.g., Fog, Clear, Snow, Rain)

## Analysis Performed

The `weather_analysis.py` script performs the following analyses:

1.  **Unique Wind Speed Values**: Identifies all unique wind speeds recorded in the dataset.
2.  **Count of Clear Weather**: Counts how many times the weather condition was 'Clear'.
3.  **Wind Speed at 4 km/h**: Filters and displays records where the wind speed was exactly 4 km/h.
4.  **Null Value Check**: Checks for and reports the sum of null values in each column.
5.  **Mean Visibility**: Calculates the average visibility across all records.
6.  **Standard Deviation of Pressure**: Computes the standard deviation of atmospheric pressure.
7.  **Variance of Relative Humidity**: Determines the variance of the relative humidity.
8.  **Snow Instances**: Retrieves all records where 'Snow' is present in the weather condition.
9.  **Fog Instances**: Filters and displays records where the weather condition is 'Fog'.
10. **High Wind and Specific Visibility**: Finds records where wind speed is greater than 24 km/h AND visibility is exactly 25 km.
11. **Mean by Weather Condition**: Calculates the mean of all numerical columns, grouped by each unique 'Weather Condition'.
12. **Maximum by Weather Condition**: Calculates the maximum of all numerical columns, grouped by each unique 'Weather Condition'.
13. **Clear Weather OR High Visibility**: Filters records where the 'Weather Condition' is 'Clear' OR 'Visibility_km' is greater than 40 km.
14. **Complex Filter**: Filters records where (('Weather Condition' is 'Clear' AND 'Rel Hum_%' is greater than 50) OR 'Visibility_km' is greater than 40).
