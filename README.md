# Analyzing Wildfire Activities in Australia and Creating a Dashboard

## Overview

This project analyzes historical wildfire data in Australia, focusing on trends, patterns, and insights using Python data science tools. The analysis is performed in a Jupyter notebook and includes a variety of visualizations to help understand the data and communicate findings effectively.

## Dataset

The dataset used is the "Historical Wildfires" dataset, which contains daily records of wildfire activities in Australia from 2005 onwards. The data includes:

- **Region**: One of seven Australian regions
- **Date**: Date of record (UTC)
- **Estimated_fire_area**: Daily sum of estimated fire area (km²)
- **Mean_estimated_fire_brightness**: Daily mean fire brightness (Kelvin)
- **Mean_estimated_fire_radiative_power**: Daily mean radiative power (MW)
- **Mean_confidence**: Daily mean confidence for fire detection
- **Std_confidence**: Standard deviation of confidence
- **Var_confidence**: Variance of confidence
- **Count**: Number of pixels flagged as fire
- **Replaced**: Indicates if data was replaced with higher quality data

## Project Structure

- **Importing Libraries**: All required libraries (pandas, numpy, seaborn, matplotlib, folium) are imported at the start for data manipulation and visualization.
- **Data Loading**: The dataset is loaded directly from a URL using pandas.
- **Data Cleaning & Feature Engineering**: The 'Date' column is converted to datetime, and new columns for 'Year' and 'Month' are extracted for time-based analysis.

## Analysis & Visualizations

### 1. Data Exploration

- **Display Sample Rows**: The first few rows of the dataset are displayed to understand its structure.
- **Column Names & Data Types**: The columns and their data types are checked to ensure correct data handling.
- **Datetime Conversion**: The 'Date' column is converted to datetime, and 'Year' and 'Month' columns are created for temporal analysis.

### 2. Trend Analysis

- **Average Estimated Fire Area Over Time**: A line plot shows how the average estimated fire area changes by year. This helps identify long-term trends and periods of increased wildfire activity.
- **Monthly Trends During Peak Years**: By grouping data by both year and month, a more granular line plot reveals seasonal or monthly patterns, especially during peak wildfire years.

### 3. Regional Analysis

- **Distribution of Mean Estimated Fire Brightness by Region**: A bar plot (using seaborn) compares the mean fire brightness across regions, highlighting which areas experience more intense fires.
- **Unique Regions**: The unique region names are listed to confirm the scope of the analysis.

### 4. Proportion Analysis

- **Pie Chart of Fire Pixel Counts by Region**: A pie chart visualizes the proportion of fire-flagged pixels in each region, showing which regions are most affected. To avoid overlapping labels, a legend is used to display percentages clearly.

### 5. Distribution Analysis

- **Histogram of Mean Estimated Fire Brightness**: A histogram shows the distribution of fire brightness values, helping to identify common intensity levels and outliers.
- **Stacked Histogram by Region**: A stacked histogram (with seaborn) visualizes how fire brightness is distributed across different regions, revealing regional differences in fire intensity.

### 6. Correlation Analysis

- **Scatter Plot: Radiative Power vs. Confidence**: A scatter plot explores the relationship between mean estimated fire radiative power and mean confidence, helping to understand if more powerful fires are detected with higher confidence.

### 7. Geospatial Visualization

- **Folium Map of Regions**: An interactive map of Australia is created using Folium, with each region marked by a colored circle. This provides a spatial context for the analysis and helps visualize the geographic distribution of wildfire activity.

## Reasoning Behind Each Analysis

- **Trend and Seasonality**: Understanding how fire activity changes over time and by season is crucial for resource planning and risk assessment.
- **Regional Differences**: Identifying which regions are most affected helps target prevention and mitigation efforts.
- **Intensity and Distribution**: Analyzing fire brightness and radiative power provides insight into the severity of wildfires.
- **Proportion and Correlation**: Pie charts and scatter plots help quantify the impact and explore relationships between variables.
- **Geospatial Context**: Mapping the data makes it easier to communicate findings to stakeholders and the public.

## Tools Used

- **pandas**: Data loading, cleaning, and manipulation
- **numpy**: Numerical operations
- **matplotlib & seaborn**: Data visualization (line plots, bar plots, histograms, scatter plots, pie charts)
- **folium**: Interactive mapping

## How to Run

1. Install the required libraries (see the notebook for pip commands).
2. Open the notebook in VS Code or Jupyter.
3. Run each cell in order to reproduce the analysis and visualizations.

## Conclusion

This project provides a comprehensive analysis of wildfire activity in Australia, combining statistical, visual, and geospatial techniques to uncover trends, patterns, and insights. The approach can be adapted to similar datasets for other regions or hazards.

# Practice-Assignment-Analyzing-wildfire-activities-in-Australia-and-creating-dashboard
