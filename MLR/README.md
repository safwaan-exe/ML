# 🧠 Student Performance Prediction using Multiple Linear Regression

## 📋 Project Overview
This project applies a **Multiple Linear Regression** model to predict a student’s **Performance Index** based on several academic and lifestyle factors such as study hours, previous scores, sleep hours, extracurricular participation, and practice tests attempted.

The model is built, trained, and evaluated using Python and Scikit-Learn in Google Colab.

---

## 🚀 Objectives
- Analyze how various factors influence student performance.
- Build and train a Multiple Linear Regression model.
- Evaluate model accuracy using **R²** and **RMSE** metrics.
- Visualize relationships, coefficients, and best-fit lines.
- Predict performance for a new student input.

---

## 🧰 Technologies Used
| Category | Tools |
|-----------|--------|
| Programming | Python |
| Libraries | Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn |
| Environment | Google Colab / Jupyter Notebook |
| Visualization | Matplotlib, Seaborn |

---

## 🗂️ Dataset Description
The dataset `Student_Performance.csv` contains the following columns:

| Feature | Description |
|----------|-------------|
| `Hours Studied` | Daily average study time (in hours) |
| `Previous Scores` | Average of past academic scores (%) |
| `Extracurricular Activities` | Participation status (Yes = 1, No = 0) |
| `Sleep Hours` | Average daily sleep hours |
| `Sample Question Papers Practiced` | Number of papers solved |
| **Target → `Performance Index`** | Overall predicted academic performance (output variable) |

---

## 🧮 Workflow
1. **Import Libraries**  
   Load all required Python libraries.

2. **Data Preparation**  
   - Load dataset  
   - Encode categorical variables (`Yes/No → 1/0`)  
   - Define features `X` and target `y`

3. **Train-Test Split**  
   Split data (75% train, 25% test).

4. **Model Training**  
   Fit a `LinearRegression()` model from `sklearn`.

5. **Predictions & Evaluation**  
   Compute:
   - R² (coefficient of determination)  
   - RMSE (root mean squared error)

6. **Coefficients & Interpretation**  
   Display feature coefficients and intercept.

7. **Visualization**  
   - Feature coefficient bar chart  
   - Actual vs Predicted scatter plot  
   - Best-fit regression line for each feature

8. **Predict for a New Student**  
   Input new student details and generate predicted performance.

---

## 📊 Model Performance (Example Results)
| Metric | Train | Test |
|--------|--------|------|
| R² Score | 0.98 | 0.98 |
| RMSE | 2.03 | 2.07 |

*(Values vary depending on dataset)*

---

## 🧩 Key Insights
- Study hours and previous scores show the highest positive correlation with performance.
- Extracurricular activities also contribute moderately.
- Sleep hours beyond optimal range may slightly reduce performance.

---

## 🧠 Future Improvements
- Implement feature scaling (StandardScaler).
- Detect and handle outliers using IQR or robust regressors.
- Compare with other models (Decision Tree, Random Forest, SVR).
- Deploy as a web app using Streamlit or Flask.
