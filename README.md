Car Price Prediction

Feature engineering and machine learning modeling on a real-world vehicle dataset.

Overview

A supervised regression workflow predicting used-car prices based on technical, numerical, and categorical attributes. Project emphasizes data cleaning, exploratory analysis, feature engineering, and model comparison.

Key Steps

Data Cleaning

Handled missing values in numerical and categorical fields.

Removed duplicate entries.

Treated outliers in Year, Engine, Selling Price, and KM Driven using IQR-based filtering.

Exploratory Analysis

Identified Year and Engine as strongest predictors of price.

Detected left-skew in Mileage and Year distributions.

Found severe skew in KM Driven and Selling Price.

Strong correlations:

Positive — Engine, Year, Seats.

Negative — KM Driven.

Categorical variables required encoding (Fuel Type, Transmission, Owner, etc.).

Feature Engineering

Log-transformed heavily skewed numerical features.

One-hot encoded categorical variables.

Standardized numerical features for linear models.

Removed features with multicollinearity or negligible predictive power.

Modeling

Compared multiple regression models: Linear Regression, Random Forest, Gradient Boosting, and XGBoost.

Evaluated using MAE, RMSE, and 
𝑅
2
R
2
.

Random Forest and XGBoost delivered the highest predictive accuracy.

Results

Achieved stable performance across train/test splits.

Feature importance: Year, Engine, KM Driven, Fuel Type, Transmission.

Files
01-eda-car-price-prediction.ipynb
02-fe-modeling-car-price-prediction.ipynb — full workflow: preprocessing → EDA → feature engineering → modeling.


Tech Stack

Python, Pandas, NumPy

Scikit-Learn

XGBoost

Matplotlib, Seaborn

Summary

A compact regression project demonstrating structured preprocessing, exploratory analysis, and model evaluation suitable for a professional ML portfolio.
