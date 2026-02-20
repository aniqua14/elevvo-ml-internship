🛒 Walmart Sales Forecasting
📌 Project Overview

This project focuses on forecasting weekly retail sales using historical Walmart store data. The dataset was provided in multiple files and merged to create a comprehensive forecasting dataset.

The goal is to compare different machine learning models and determine the best-performing approach for sales prediction.

📊 Dataset

Dataset Source: Kaggle – Walmart Sales Forecast

Files Used:

train.csv

features.csv

stores.csv

Merged using:

Store

Date

IsHoliday

🔧 Feature Engineering

Converted Date to datetime format

Extracted:

Year

Month

Week

Filled missing MarkDown values with 0

One-hot encoded Store Type

Created time-series features:

Lag_1 (previous week sales)

Rolling_Mean_4 (4-week moving average)

Time-based split was used:

Training: Data before 2012

Testing: Data from 2012

🤖 Models Implemented

Linear Regression

Random Forest Regressor

XGBoost Regressor

Evaluation Metrics:

MAE (Mean Absolute Error)

RMSE (Root Mean Squared Error)

R² Score

📈 Model Performance

| Model             | R² Score |
| ----------------- | -------- |
| Linear Regression | 0.960    |
| Random Forest     | 0.974    |
| XGBoost           | 0.975    |

🏆 Final Conclusion

XGBoost achieved the highest R² score (0.975), making it the best-performing model for this forecasting task. Ensemble tree-based models outperformed linear regression due to their ability to capture nonlinear relationships in retail sales data.

🛠 Tools & Libraries

Python

Pandas

NumPy

Scikit-learn

XGBoost

Matplotlib

📌 Key Learning Outcomes

Time-series feature engineering

Avoiding data leakage

Time-based train-test split

Model comparison and evaluation

Feature importance analysis
