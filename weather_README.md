# Weather Prediction and Advisory System

A machine learning project that forecasts rainfall using multiple classification algorithms with interactive dashboards for weather data visualization.

## Overview

This project builds a rainfall prediction system using Australia's weather dataset. It compares three ML models — Logistic Regression, Decision Tree, and XGBoost — to identify the best performing model for accurate rain forecasting.

## Features

- **Data Cleaning** — Handles missing values using median/mode imputation for numerical and categorical features
- **EDA & Visualization** — Interactive dashboards using Plotly to explore weather patterns and correlations
- **Feature Selection** — SelectKBest with chi2 scoring to identify top 15 most impactful features
- **Model Comparison** — Trains and evaluates Logistic Regression, Decision Tree, and XGBoost side by side
- **Real-time Prediction** — Accepts weather inputs and returns rain probability instantly

## Dataset

- 145,000+ weather records from Australia (Kaggle)
- 23 features including temperature, humidity, wind speed, pressure, rainfall
- Target: RainTomorrow (Yes/No)

## Tech Stack

- Python
- Pandas, NumPy
- Plotly, Seaborn, Matplotlib
- Scikit-learn (Logistic Regression, Decision Tree, Feature Selection)
- XGBoost

## Results

- XGBoost achieved best performance across accuracy and AUC Score
- Feature importance analysis identified Humidity3pm and Pressure3pm as top predictors
- Interactive confusion matrix and model comparison dashboard included

## How to Run

1. Clone the repository
2. Install dependencies:
```
pip install pandas numpy matplotlib seaborn plotly scikit-learn xgboost
```
3. Place `weatherAUS.csv` in the project folder
4. Open and run `weather_prediction.ipynb` in Jupyter Notebook or Google Colab
