# ❤️ Heart Disease Prediction using Classification Algorithms

A machine learning project focused on predicting the presence of heart disease using clinical and demographic data along with classification models.

---

## 📌 Project Overview

This project builds an end-to-end pipeline: ingestion of patient data (e.g., age, blood pressure, cholesterol, chest pain type, maximum heart rate), exploratory data analysis (EDA) to uncover patterns, feature engineering (encoding, normalization), training classification models, and evaluating their performance. The aim is to accurately classify whether a patient has heart disease and offer insights into major risk factors.

---

## 🧰 Tech Stack

* **Language:** Python
* **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn
* **Environment:** Jupyter Notebook / Google Colab

---

## 🔄 Workflow Summary

### 1. Data Collection

Dataset includes clinical and demographic features such as: age, sex, chest pain type, resting blood pressure, serum cholesterol, fasting blood sugar, maximum heart rate achieved, exercise-induced angina, old peak ST depression, slope of peak exercise ST segment, number of major vessels, thalassemia indicator, and target label indicating presence or absence of heart disease.

### 2. Exploratory Data Analysis (EDA)

* Distribution of patients with and without heart disease
* Feature distributions (age, cholesterol, max heart rate) by class
* Correlation matrix and heatmap to identify relationships among features
* Detection of missing values, outliers, skewness and class imbalance

### 3. Feature Engineering

* Encoding categorical features (e.g., chest pain type, thal) into numeric form
* Handling missing values (imputation)
* Scaling numerical features (standardization) for model compatibility
* Constructing interaction features if relevant (e.g., age × cholesterol)
* Splitting dataset into training and test sets with stratified sampling

### 4. Modeling

Classification algorithms implemented:

* **Logistic Regression** (baseline)
* **Random Forest Classifier** (strong performer)
* **Support Vector Machine** or **XGBoost** for improved performance

### 5. Evaluation

Metrics used to evaluate model performance:

* Accuracy
* Precision, Recall, F1-Score
* Confusion Matrix
* ROC–AUC

**Result:** The best classification model achieved high accuracy and recall, indicating the system’s capability to correctly identify patients at risk of heart disease.

### 6. Prediction & Insights

* Generated predictions on unseen patient profiles
* Analyzed feature importance: e.g., chest pain type, maximum heart rate, old peak ST depression emerged as influential
* Provided actionable insights: focusing on high-risk patients, early screening of key clinical indicators

---

## 📁 Project Structure

```
Heart-Disease-Prediction/
│── data/
│── notebooks/
│── src/
│── README.md
│── requirements.txt
```

---

## 📈 Key Findings

* Chest pain type and max heart rate were among the most significant predictors of heart disease
* Feature standardization and encoding were essential for improved model performance
* Classification models like Random Forest delivered reliable predictions in this healthcare context
* The pipeline supports early detection efforts by ranking patients based on risk

---

## 🚀 Future Improvements

* Expand dataset to include larger and more diverse patient populations and additional clinical indicators
* Deploy the model via a web application (Flask/Streamlit) for clinical use and real-time screening
* Use explainability tools such as SHAP or LIME to interpret predictions for healthcare professionals
* Evaluate model fairness and bias across different demographics (gender, age, ethnicity)
* Introduce time-series or longitudinal patient data to predict disease progression rather than just presence

---
