# Weather Trend Forecasting

This project is a comprehensive weather forecasting and climate analysis pipeline built for the **PM Accelerator Technical Assessment**. It leverages global weather data to uncover meaningful trends, detect anomalies, and forecast future temperatures using a combination of statistical and machine learning models.

##  Objective

To analyze the [Global Weather Repository](https://www.kaggle.com/datasets/nelgiriyewithana/global-weather-repository) dataset and forecast future weather trends using both basic and advanced data science techniques.

## Project Highlights

###  Data Preprocessing
- Cleaned missing values, handled outliers, and normalized key numerical features
- Converted timestamp fields into usable datetime formats
- Conducted sanity checks on global temperature ranges and distributions

###  Exploratory Data Analysis (EDA)
- Explored correlations between weather variables (e.g., temperature, humidity, pollution)
- Visualized global temperature variations across cities and continents
- Plotted time series trends and seasonal patterns

###  Anomaly Detection
- Implemented rolling mean and standard deviation logic to flag temperature anomalies per city
- Visualized anomalies using time series plots

###  Forecasting Models
Forecasted 30-day temperature trends using 3 distinct approaches:
- **Prophet** for Yerevan  
- **ARIMA** for Tirana  
- **ETS (Holt-Winters)** for Kabul  

Also created an **ensemble average** for all 3 cities.

###  Model Evaluation
Each model was evaluated using:
- **Mean Absolute Error (MAE)**
- **Root Mean Square Error (RMSE)**

Prophet (Yerevan):  
- MAE: `6.0674`  
- RMSE: `6.7243`  

ETS (Kabul):  
- MAE: `0.0474`  
- RMSE: `0.0503`  

ARIMA (Tirana):  
- MAE: `0.0487`  
- RMSE: `0.0555`  

###  Climate & Environmental Insights
- Compared long-term temperature patterns across multiple regions
- Analyzed air quality metrics (e.g., PM2.5, CO) and their relationships to temperature
- Ranked cities with high or low pollution alongside temperature fluctuations

###  Spatial Analysis
- Plotted geospatial temperature distributions using Plotly
- Visualized pollution data and weather patterns across latitude and longitude

###  Feature Importance
- Trained a regression model to rank the most influential features on temperature
- Top predictors included: `feels_like_celsius`, `temperature_fahrenheit`, and `feels_like_fahrenheit`

---



