# MSCS-634 Lab 1 - Data Visualization, Data Preprocessing, and Statistical Analysis

**Dataset:** [Global Air Quality Dataset](https://www.kaggle.com/datasets/waqi786/global-air-quality-dataset)

---

## Purpose  
This lab explores global air quality measurements using Python. The focus is on visualization, preprocessing (cleaning, outlier detection, scaling), and statistical analysis (central tendency, dispersion, correlation).

---

## Key Insights  
- The scatter plot of PM2.5 vs. AQI revealed a strong positive correlation, confirming that fine particulate matter (PM2.5) is a major determinant of air quality. Most regions clustered in the moderate pollution range, while a few outliers indicated severe pollution events.  
- The AQI histogram displayed a near-normal distribution centered between 60 and 80, suggesting that most cities maintain moderate air quality, with relatively few extreme pollution or exceptionally clean readings.  
- Statistical measures such as mean, median, and standard deviation supported these findings—AQI values were evenly distributed without heavy skewness, and pollutant variables showed consistent relationships across countries.  
- Correlation analysis further validated that PM2.5 and PM10 had the strongest influence on AQI, while weather features like humidity and wind speed showed weaker correlations.

---

## Challenges & Decisions  
- The dataset did not contain a direct AQI column, so a derived AQI metric was created using a weighted combination of pollutant concentrations.  
- Several columns contained missing values, which were handled using median imputation to preserve data integrity.  
- Some extreme outliers were detected in PM2.5 values; the Interquartile Range (IQR) method was applied to remove them and improve model consistency.  
- To optimize performance and visualization clarity, a 20% sample of the cleaned dataset was used for the final analysis.  

---
