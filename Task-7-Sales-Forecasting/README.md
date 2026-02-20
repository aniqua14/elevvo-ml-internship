# Task 7: Walmart Sales Forecasting

## 📌 Overview
This project focuses on building an end-to-end machine learning pipeline to forecast weekly retail sales using historical Walmart store data. The task is formulated as a regression problem and reflects real-world retail demand forecasting challenges used in business planning and inventory optimization systems.

---

## 📊 Dataset
- Source: Kaggle – Walmart Sales Forecast Dataset  
- Target Variable: `Weekly_Sales`  
- The dataset was provided in multiple files and merged using:
  - `Store`
  - `Date`
  - `IsHoliday`

The final dataset combines store-level, economic, promotional, and time-based features.

---

## ⚙️ Workflow
1. Data loading and exploration  
2. Merging `train.csv`, `features.csv`, and `stores.csv`  
3. Handling missing values (MarkDown columns filled with 0)  
4. Converting `Date` to datetime format  
5. Time feature extraction:
   - `Year`  
   - `Month`  
   - `Week`  
6. Feature engineering:
   - `Lag_1` (previous week sales)  
   - `Rolling_Mean_4` (4-week moving average)  
7. One-hot encoding categorical variables  
8. Time-based train-test split:
   - Training: Data before 2012  
   - Testing: Data from 2012  
9. Model training:
   - Linear Regression  
   - Random Forest Regressor  
   - XGBoost Regressor  
10. Model evaluation using:
   - MAE (Mean Absolute Error)  
   - RMSE (Root Mean Squared Error)  
   - R² Score  
11. Model comparison and feature importance analysis  

---

## 🤖 Models Implemented
- Linear Regression  
- Random Forest Regressor  
- XGBoost Regressor  

---

## 📈 Model Performance

| Model | R² Score |
|-------|----------|
| Linear Regression | 0.960 |
| Random Forest | 0.974 |
| XGBoost | 0.975 |

---

## 🧠 Key Learnings
- Time-based splitting prevents data leakage in forecasting tasks.
- Feature engineering (lag features and rolling averages) significantly improves performance.
- Ensemble tree-based models capture nonlinear sales patterns better than linear regression.
- Multiple evaluation metrics provide deeper insight into forecasting performance.

---

## 🛠 Tools & Libraries
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- XGBoost  
- Matplotlib  

---

## 📁 Files
- `Sales_Forecasting.ipynb` – Complete implementation and analysis  
- `README.md` – Project documentation  

---

## ✅ Conclusion
This project demonstrates a complete end-to-end sales forecasting workflow including multi-source data integration, time-series feature engineering, regression model comparison, and performance evaluation. XGBoost achieved the highest R² score, making it the best-performing model for this task.
