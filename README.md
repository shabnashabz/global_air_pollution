# Global Air Pollution Data Analysis 
## Overview
This project focuses on the analysis of Global Air Pollution using a dataset that includes air quality indices (AQI) for various pollutants across different countries. The goal of this project is to examine the air pollution levels and understand the global trends, with a special emphasis on the most polluted countries.

This analysis was performed using Python and popular data visualization libraries like Matplotlib and Seaborn.


## Key Objectives
Analyze air quality data to understand the pollution levels for different pollutants like CO, Ozone, NO2, and PM2.5.
Visualize the top 10 most polluted countries and key AQI statistics.
Summarize air quality index trends across countries and pollutants.
## Dataset
Filename: Global Air Pollution Dataset
Source: Kaggle
Data fields:
Country: The country where air quality is measured.
Year: The year of the measurement.
CO AQI Value: Air Quality Index value for Carbon Monoxide.
Ozone AQI Value: Air Quality Index value for Ozone.
NO2 AQI Value: Air Quality Index value for Nitrogen Dioxide.
PM2.5 AQI Value: Air Quality Index value for particulate matter (PM2.5).
## Tools & Technologies
Python: Programming language used for data analysis.
Pandas: Library used for data manipulation and cleaning.
Matplotlib & Seaborn: Visualization libraries for creating insightful charts and graphs.
Jupyter Notebook: For interactive data analysis.
## Key Steps in the Analysis:
Data Loading:

```python

df = pd.read_csv('/kaggle/input/global-air-pollution-dataset/global air pollution dataset.csv')
df.head()
```
## Data Exploration:

Use df.info() to explore the structure of the dataset.
Visualize missing data, data types, and basic statistics of the dataset.
Data Cleaning:

Handle any missing values and outliers in the dataset.
Normalize data for easy comparison.
## Data Visualization:

A summary statistics plot was created to show the highest, lowest, and average AQI values for different pollutants.
The top 10 most polluted countries were identified based on AQI values.
Example visualizations:

```python

sns.barplot(x='Country', y='AQI Value', data=top_polluted_countries)
plt.title('Top 10 Most Polluted Countries')
```
```python

sns.catplot(x='Statistic', y='AQI Value', hue='Pollutant', data=summary_stats)
plt.title('Summary Statistics of Air Quality Indices')
```
## Insights Gained:

Republic of Korea ranks highest in terms of AQI, followed by Bahrain and Mauritania.
CO and PM2.5 are the most significant pollutants, contributing to the highest AQI values in several countries.
A clear trend of increasing AQI values over the years, indicating worsening air quality in some regions.
## Example Visualizations
Summary Statistics of Air Quality Indices

Highest, lowest, and average AQI values for pollutants like CO, Ozone, NO2, and PM2.5.
Top 10 Most Polluted Countries

Countries with the highest AQI values are visualized to highlight global pollution levels.
## Conclusion
The data analysis showcases the severity of air pollution in various parts of the world, with significant AQI levels for pollutants like CO and PM2.5. Countries in the Middle East and Asia are among the most affected by air pollution, emphasizing the need for stricter environmental regulations and sustainable practices.
