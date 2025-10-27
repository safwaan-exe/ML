# 🕵️‍♂️ Credit Card Fraud Detection using Random Forest Classifier

## 📘 Overview
This project implements a **Random Forest Classifier** to detect fraudulent credit card transactions.  
The dataset is highly **imbalanced**, so both **original** and **SMOTE-balanced** versions were tested to compare performance.

---

## ⚙️ Model Setup
- **Algorithm Used:** Random Forest Classifier  
- **Techniques:** SMOTE (Synthetic Minority Oversampling Technique)  
- **Libraries:** `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`

---

## 📊 Model Performance

| Dataset Type | Accuracy | ROC-AUC Score | Precision (Class 1) | Recall (Class 1) | F1-Score (Class 1) |
|---------------|-----------|----------------|----------------------|------------------|--------------------|
| Without SMOTE | 0.9995 | 0.9239 | 0.97 | 0.73 | 0.83 |
| With SMOTE | 0.9994 | **0.9656** | 0.91 | **0.76** | **0.83** |

---

## 📈 Insights
- **SMOTE improved model recall** and ROC-AUC score, helping the model better detect fraudulent cases.  
- Both models achieved **extremely high accuracy**, expected due to dataset imbalance.  
- **Top 5 important features:**  
  - `V14` → 0.1956  
  - `V10` → 0.1139  
  - `V12` → 0.0998  
  - `V4` → 0.0928  
  - `V17` → 0.0901  
- **V14** was the most influential feature in detecting fraud.  
- **Hyperparameter tuning** was not performed, as the default model already yielded strong results.  
  - It can be explored in the future to further improve recall.

---

## 🔍 Sample Prediction
```python
Sample Transaction: {'Time': -0.7077, 'V1': 1.2288, 'V2': -0.0634, ..., 'Amount': -0.3128}
Predicted Class: Legitimate
Confidence of Fraud: 0.00%
Confidence of Legitimate Transaction: 100.00%

