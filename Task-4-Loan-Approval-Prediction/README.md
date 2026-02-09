# Task 4: Loan Approval Prediction

## 📌 Overview
This project focuses on building an end-to-end machine learning pipeline to predict loan approval decisions based on applicant demographic and financial information. The task is formulated as a binary classification problem and reflects real-world challenges faced in financial risk assessment systems.

---

## 📊 Dataset
- Source: Kaggle – Loan Prediction Dataset
- Target Variable: `Loan_Status`
  - 1 → Loan Approved
  - 0 → Loan Rejected
- The dataset contains both numerical and categorical features and exhibits class imbalance.

---

## ⚙️ Workflow
1. Data loading and exploration
2. Handling missing values
3. Encoding categorical variables
4. Feature scaling
5. Train-test split with stratification
6. Model training:
   - Logistic Regression
   - Decision Tree Classifier
7. Model evaluation using:
   - Accuracy
   - Precision, Recall, F1-score
   - Confusion Matrix
8. Handling class imbalance using SMOTE
9. Model comparison and interpretation

---

## 🧠 Key Learnings
- Accuracy alone is not sufficient for evaluating models on imbalanced datasets.
- Recall for the minority class (loan rejection) is critical in financial decision-making.
- SMOTE improves minority class detection at the cost of slight accuracy reduction.
- Model choice should align with business objectives such as risk tolerance and customer experience.

---

## 🛠 Tools & Libraries
- Python
- Pandas, NumPy
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Matplotlib, Seaborn

---

## 📁 Files
- `Loan_Approval_Prediction.ipynb` – Complete implementation and analysis
- `README.md` – Project documentation

---

## ✅ Conclusion
This project demonstrates a practical approach to loan approval prediction by combining data preprocessing, model evaluation beyond accuracy, and imbalance handling techniques. The results highlight the importance of risk-aware modeling in real-world financial applications.
