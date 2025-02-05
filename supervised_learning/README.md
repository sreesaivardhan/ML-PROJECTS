# Weather Data Prediction Using Linear Regression  

## Overview  
This project applies **Supervised Learning** techniques, specifically **Linear Regression**, to predict precipitation levels based on various weather attributes. The dataset used contains historical weather data, which is cleaned and preprocessed before training a machine learning model.  

## Machine Learning Approach  
- **Supervised Learning**: The model is trained on labeled weather data to predict precipitation.  
- **Linear Regression**: Used to model the relationship between input weather features (temperature, humidity, wind speed, etc.) and precipitation.  

## Steps in the Code  

### 1. Data Cleaning & Preprocessing  
- Reads weather data from `weather.csv` using **pandas**.  
- Drops unnecessary columns (`Events`, `Date`, etc.).  
- Replaces missing or trace values ('T' and '-') with `0.0`.  
- Saves the cleaned dataset as `weather_final.csv`.  

### 2. Train the Linear Regression Model  
- Defines **X (input features)** and **Y (target: PrecipitationSumInches)**.  
- Trains a **Linear Regression** model using **Scikit-Learn**.  

### 3. Making Predictions  
- Predicts precipitation for a given set of weather attributes.  

### 4. Data Visualization  
- **Precipitation Trend Graph**: Shows precipitation levels over time.  
- **Feature Correlation Graphs**: Visualizes how weather attributes influence precipitation.  

## Technologies Used  
- Python  
- Pandas (Data Handling)  
- NumPy  
- Scikit-Learn (Machine Learning)  
- Matplotlib (Data Visualization)  

## How to Run  
1. Install dependencies:  
   ```bash
   pip install pandas numpy scikit-learn matplotlib
