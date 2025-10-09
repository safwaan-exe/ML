# Titanic Survival Prediction Using Logistic Regression

## Project Overview
This project implements **Logistic Regression** to predict whether a passenger survived the Titanic disaster based on features like age, sex, passenger class, and other personal attributes.  

**Objective:**  
Classify passengers as `Survived` (1) or `Not Survived` (0) using historical Titanic data.

---

## Libraries & Technologies Used
- **Python** – Programming language  
- **Pandas** – Data manipulation and analysis  
- **NumPy** – Numerical computations  
- **Scikit-learn** – Machine learning algorithms  
- **Matplotlib & Seaborn** – Data visualization  
- **Jupyter Notebook / Colab** – Project development environment  

---

## Dataset
**Source:** Kaggle – [Titanic Survival Prediction Dataset for ML](https://www.kaggle.com/datasets/yasserh/titanic-dataset))  
**Number of samples:** 891  
**Target variable:** `Survived` (0 = No, 1 = Yes)  

**Key Features:**
- `Pclass` – Passenger class (1, 2, 3)  
- `Sex` – Gender of passenger  
- `Age` – Age in years  
- `SibSp` – Number of siblings/spouses aboard  
- `Parch` – Number of parents/children aboard  
- `Fare` – Passenger fare  
- `Embarked` – Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)  

**Preprocessing Steps:**
- Filled missing values for `Age` and `Embarked`  
- Converted categorical variables (`Sex`, `Embarked`) to numerical values  
- Dropped irrelevant columns: `Cabin`, `Ticket`, `Name`  
- Split dataset into training and testing sets  

---

## Methodology
1. **Exploratory Data Analysis (EDA)** – Visualize distributions, correlations, and identify patterns.  
2. **Feature Engineering** – Encode categorical variables, handle missing values.  
3. **Model Building** – Train Logistic Regression model using `scikit-learn`.  
4. **Evaluation** – Evaluate model with accuracy, confusion matrix, precision, recall, F1-score.  

---

## Results

| Metric                 | Value        |
|------------------------|--------------|
| Training Accuracy      | 0.7935       |
| Testing Accuracy       | 0.7877       |
| Precision (Survived)   | 0.8727       |
| Recall (Survived)      | 0.8000       |
| F1-Score (Survived)    | 0.8348       |
| ROC-AUC Score          | 0.8390       |
| GridSearchCV Accuracy  | 0.8034       |


---

## Conclusion
The Logistic Regression model is able to predict Titanic passenger survival with reasonable accuracy. Important features influencing survival include `Sex`, `Pclass`, and `Age`. Model performance can be further improved using techniques like hyperparameter tuning, feature selection, or using more advanced classifiers such as Random Forest or XGBoost.  
