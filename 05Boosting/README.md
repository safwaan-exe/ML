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

## 🧾 Evaluation Outputs

### Tuned Random Forest
🎯 Train Accuracy: 100.0%
🎯 Test Accuracy: 92.27%
✅ Best Parameters: {'n_estimators': 500, 'min_samples_split': 2, 'min_samples_leaf': 2, 'max_features': 'log2', 'max_depth': 15}
✅ Best Cross-Validation Accuracy: 93.41%


### Tuned XGBoost
🎯 Train Accuracy: 95.23%
🎯 Test Accuracy: 91.36%
✅ Best Parameters: {'subsample': 0.8, 'reg_lambda': 1, 'reg_alpha': 0.5, 'n_estimators': 100, 'max_depth': 5, 'learning_rate': 0.01, 'gamma': 0.5, 'colsample_bytree': 0.6}
✅ Best Cross-Validation Accuracy: 93.98%


---

## ✅ Final Conclusion
- **Best Performing Model:** Tuned **Random Forest**  
  - Highest test accuracy: **92.27%**  
  - Slightly better generalization on holdout data.  
- **Alternative Choice:** Tuned **XGBoost**  
  - Excellent cross-validation stability (**93.98%**).  
  - Slightly lower test accuracy but more robust and less overfitting.

---

## 🚀 Future Improvements
- Use **SMOTE / ADASYN** for imbalanced data handling.
- Implement **LightGBM** or **CatBoost** for faster training.
- Apply **SHAP / LIME** for model explainability.
- Create a **Streamlit / Flask** web app for interactive stress prediction.
- Deploy the final model with monitoring and versioning (MLOps pipeline).

---

## 🗂 Project Structure
.
├── data/
│ ├── raw/ # Original dataset
│ └── processed/ # Cleaned dataset
├── notebooks/
│ ├── 01_EDA.ipynb
│ ├── 02_Preprocessing.ipynb
│ ├── 03_RandomForest.ipynb
│ └── 04_XGBoost.ipynb
├── models/
│ ├── rf_tuned.pkl
│ └── xgb_tuned.pkl
├── src/
│ ├── data_preprocess.py
│ └── model_utils.py
├── README.md
└── requirements.txt


---

## 👨‍💻 Author
**Safwaan Siddiqui**  
B.Tech CSE (AIML) | Manipal University Jaipur  
GitHub: [@safwaan-exe](https://github.com/safwaan-exe)

---
