# Air Quality Assessment and Sensor Reliability Analysis

This repository contains a comprehensive analysis of air quality data and the performance of low-cost gas sensors compared to reference laboratory analyzers. The project focuses on identifying pollution patterns, seasonal trends, and the reliability of various sensor technologies.

---

## 📊 Project Overview

The analysis uses the **AirQualityUCI dataset**, containing 9,357 instances of hourly averaged responses from an array of 5 metal oxide chemical sensors. The project is divided into three main phases:

1. 
**Data Pre-processing**: Cleaning, handling missing values (indicated by -200 in the raw data), and feature engineering.


2. 
**Exploratory Data Analysis (EDA)**: Visualizing diurnal and monthly trends of pollutants like , , and .


3. 
**Sensor Reliability Analysis**: Comparing low-cost sensor outputs against Ground Truth (GT) reference data to determine accuracy and error rates.



---

## 🔍 Key Insights

### 1. Pollution Patterns

* 
**Diurnal Trends**: CO levels exhibit a bimodal distribution with peaks in the morning and evening, directly correlating with peak traffic hours.


* 
**Seasonal Trends**:  concentrations are significantly higher in winter months and lower during summer, indicating seasonal atmospheric effects or heating-related emissions.


* 
**Pollutant Correlation**: There is a strong linear correlation between , , and , suggesting these pollutants originate from common combustion-related sources, primarily vehicle emissions.



### 2. Sensor Performance & Reliability

The analysis evaluated sensors based on their correlation with reference analyzers and their normalized error rates.

| Sensor | Performance (%) | Normalized Error | Grade |
| --- | --- | --- | --- |
| **CO Sensor (S1)** | 87.93% | 0.362 | **Best** |
| **NMHC Sensor (S2)** | 87.77% | 0.384 | **Better** |
| **NOx Sensor (S3)** | 65.57% | 1.390 | **Good** |
| **NO2 Sensor (S4)** | 15.77% | 1.070 | **Average** |

* 
**Primary Finding**: The **CO Sensor (PT08.S1)** is the most reliable, showing the highest trend accuracy and the lowest relative error.


* 
**Error Dynamics**: Sensors with lower trend accuracy consistently demonstrated higher measurement errors.



---

## 🛠️ Tech Stack

* 
**Language**: Python 


* **Libraries**:
* 
`pandas` & `numpy` for data manipulation.


* 
`matplotlib` & `seaborn` for advanced data visualization.


* 
`scipy.stats` for statistical analysis and Z-score normalization.





---

## 📈 Visualizations Included

* 
**Univariate Analysis**: Histograms of CO concentration.


* 
**Time-Series**: Daily average CO trends and diurnal variation plots.


* 
**Bivariate Analysis**: Correlation heatmaps and pairwise relationship matrices.


* 
**Composition**: Pie charts showing the relative contribution of major pollutants ( and  being the largest contributors).



---

Would you like me to generate a summary of the specific Python functions used for the sensor error calculations?
