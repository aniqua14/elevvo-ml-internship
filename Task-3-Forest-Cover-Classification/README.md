# Task 3: Forest Cover Type Classification

## 📌 Overview
This project focuses on predicting forest cover types using cartographic and environmental features. The task is formulated as a multi-class classification problem and reflects real-world applications in environmental data modeling and ecological analysis.

The objective of this project is to compare ensemble learning models and determine the most effective approach for forest cover classification in environmental data modeling applications.

---

## 📊 Dataset
- Source: Kaggle – Forest Cover Type Dataset  
- Target Variable: `Cover_Type`  
- Number of Classes: 7 forest cover types  

### Key Features Include:
- Elevation  
- Aspect  
- Slope  
- Horizontal & Vertical Distance measurements  
- Soil Type indicators  
- Wilderness Area indicators  

The dataset contains purely numerical and encoded environmental features.

---

## ⚙️ Workflow
1. Data loading and exploration  
2. Exploratory Data Analysis (EDA)  
3. Train-test split  
4. Model training:
   - Random Forest Classifier  
   - XGBoost Classifier  
5. Model evaluation using:
   - Accuracy  
   - Classification Report  
   - Confusion Matrix  
6. Model comparison  
7. Feature importance analysis  

---

## 🤖 Models Implemented
- Random Forest Classifier  
- XGBoost Classifier  

---

## 📈 Model Performance

| Model | Accuracy |
|--------|----------|
| Random Forest | 0.953 |
| XGBoost | 0.868 |

Random Forest achieved the highest classification accuracy and outperformed XGBoost in this implementation.
---

## 🧠 Key Learnings
- Random Forest demonstrated strong performance in multi-class environmental classification tasks.
- Proper label encoding is essential when using XGBoost for multi-class problems.
- Confusion matrices provide deeper insight into model performance beyond overall accuracy.
- Feature importance analysis helps interpret how environmental factors influence forest cover types.
- Ensemble tree-based methods are highly effective for structured cartographic datasets.

---

## 🛠 Tools & Libraries
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- XGBoost  
- Matplotlib  
- Seaborn  

---

## 📁 Files
- `Forest_Cover_Classification.ipynb` – Complete implementation and evaluation  
- `README.md` – Project documentation  

---

## ✅ Conclusion
This project demonstrates the effectiveness of ensemble tree-based models for multi-class environmental classification. Random Forest achieved the highest predictive accuracy (0.953), outperforming XGBoost in this implementation. The results highlight the robustness of bagging-based ensemble methods for structured cartographic data.