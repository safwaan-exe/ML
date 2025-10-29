# 🧠 Student Stress Prediction — Machine Learning Project

## 📘 Project Overview
This project analyzes factors affecting **student stress** and builds machine learning classifiers to **predict stress levels**.  
We implemented and compared **Random Forest** and **XGBoost** models, performed **hyperparameter tuning**, and produced a final model recommendation.

---

## 📂 Dataset
**Dataset Used:** [Student Stress Factors — A Comprehensive Analysis (Kaggle)](https://www.kaggle.com/datasets/rxnach/student-stress-factors-a-comprehensive-analysis)

The dataset includes demographic, academic, and lifestyle attributes of students, along with their stress levels.  
The task was converted into **binary classification**:  
- `0` → Not Stressed  
- `1` → Stressed  

---

## ⚙️ Technologies & Libraries
- **Python**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn**
- **Scikit-learn**
- **XGBoost**
- **Google Colab / Jupyter Notebook**

---

## 🧩 Project Workflow
1. **Exploratory Data Analysis (EDA)**
   - Inspected dataset shape, datatypes, null values, and distributions.
   - Checked correlations and visualized stress-level relationships.
2. **Data Preprocessing**
   - Dropped irrelevant columns (e.g., `Timestamp`, `User_ID`, etc.).
   - Encoded categorical features using `LabelEncoder`.
   - Standardized numerical features using `StandardScaler`.
   - Converted target to binary form.
3. **Train-Test Split**
   - Used `train_test_split` (80–20) with `random_state=42`.
4. **Model Training**
   - Implemented **Random Forest** and **XGBoost** classifiers.
   - Evaluated baseline performance.
5. **Hyperparameter Tuning**
   - Used `RandomizedSearchCV` for both models to find optimal parameters with 5-fold cross-validation.
6. **Evaluation Metrics**
   - Accuracy, Precision, Recall, F1-score, and Confusion Matrix.
7. **Model Comparison**
   - Compared untuned and tuned versions of both models to finalize the best performer.

---

## 📊 Model Performance Summary

| Model | Train Accuracy | Test Accuracy | CV Accuracy | Remarks |
|-------|----------------|---------------|-------------|----------|
| Random Forest (Untuned) | 100.0% | 90.91% | - | Overfitting observed |
| Random Forest (Tuned) | 100.0% | **92.27%** | 93.41% | Improved generalization |
| XGBoost (Untuned) | 100.0% | 90.91% | - | Strong baseline |
| XGBoost (Tuned) | 95.23% | 91.36% | **93.98%** | Stable & high CV performance |

---

## 🧾 Evaluation Outputs

### Tuned Random Forest

