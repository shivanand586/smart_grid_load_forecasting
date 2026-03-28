# Electric Load Forecasting using Machine Learning

## Overview
This project focuses on predicting electricity demand using historical consumption data and machine learning techniques. Accurate load forecasting is essential for efficient smart grid operation, enabling better demand-supply balance, reduced energy wastage, and improved grid stability.

---

## Objective
- Predict future electricity load using past consumption data
- Apply machine learning models to time-series forecasting
- Analyze performance of different models
- Demonstrate the importance of feature engineering in prediction tasks

---

## Dataset
- Source: UCI Electricity Load Dataset
- Contains data from 370+ smart meters
- Time resolution: 15-minute intervals
- Each column represents an individual consumer’s electricity usage

### Data Processing
- Converted timestamp to datetime format
- Set timestamp as index
- Handled missing values using forward fill
- Aggregated all meter readings to compute total grid load

---

## Feature Engineering
To capture temporal dependencies, the following features were created:

### Time-based Features
- Hour of the day
- Day of the week
- Month
- Weekend indicator

### Lag Features
- Previous time step load (lag-1)
- Previous day load (lag-24)

> These features help the model learn patterns in electricity consumption over time.

---

## Methodology
1. Data Preprocessing  
2. Feature Engineering  
3. Train-Test Split (70/30, time-based)  
4. Model Training  
5. Model Evaluation  

---

## Models Used
- Linear Regression  
- Random Forest Regressor  
- Support Vector Regression (SVR)  

---

## Evaluation Metrics
- Mean Absolute Error (MAE)  
- Root Mean Square Error (RMSE)  
- Mean Absolute Percentage Error (MAPE)  
- R² Score

---

## Key Insights
- Electricity demand follows strong daily and weekly patterns  
- Past consumption is the most important predictor  
- Simple models can perform extremely well with proper feature engineering  
