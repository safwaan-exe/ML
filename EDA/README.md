# 🧩 Project 1: Exploratory Data Analysis on Heart Disease Prediction

### 🔍 Overview
This project focuses on performing an **Exploratory Data Analysis (EDA)** on a Heart Disease dataset to understand its structure, identify data quality issues, and uncover patterns and relationships between variables. The primary goal of this analysis is to prepare the data for subsequent machine learning model building by ensuring its quality and extracting meaningful insights.

---

## 📊 Project Objectives
- Perform data cleaning and preprocessing
- Remove duplicates  
- Handle missing values and outliers  
- Univariate and Bivariate Analysis  
- Visualize key trends and metrics
- Generate actionable insights from the dataset
- Normalisation and Scaling (here we used standard scaler)
- Encoding  

---
## Dataset

The analysis uses the **Heart Dataset**, which contains features related to heart health and a binary target variable indicating the presence or absence of heart disease.

* **File Used:** `heart.csv`
* **Shape:** 1025 rows and 14 columns
* **Key Columns:** The dataset includes various medical and demographic predictors, with the **target** column being the variable of interest for prediction.

---

## Methodology: Key Steps of EDA

The Exploratory Data Analysis was performed methodically, covering essential data preprocessing and analytical steps:

1.  **Basic Data Exploration:** Checking the head, shape, data types (`info()`), and summary statistics (`describe()`) of the dataset.
2.  **Data Cleaning & Preprocessing:**
    * Removing duplicates
    * Missing value treatment
    * Outlier treatment
3.  **Feature Engineering & Scaling:**
    * Normalisation and scaling for Numerical variables
    * Encoding categorical variables (Dummy variables)
4.  **Data Analysis & Visualization:**
    * Univariate Analysis (analyzing individual variables)
    * Bivariate Analysis (analyzing relationships between two variables)
  
---

  
## 🧰 Tools & Libraries Used
| Category | Libraries |
|-----------|------------|
| Data Handling | `pandas`, `numpy` |
| Visualization | `matplotlib`, `seaborn` |
| Notebook Environment | `Google Colab` |




