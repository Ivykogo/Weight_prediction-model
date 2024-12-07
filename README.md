# Predicting Weight Using Machine Learning

## Overview
This project uses machine learning to predict a person's weight based on various features like height, BMI, calories burned, and workout type. The model is trained using **XGBoost** to make accurate predictions.

---

## Dataset
- **Features**:
  - **Height (m)**
  - **Calories Burned**
  - **Fat Percentage**
  - **BMI**
  - **Gender**
  - **Workout Type**
  - **Session Duration (hours)**
- **Target**: **Weight (kg)**
- **Size**: 973 rows, 15 columns.

---

## Steps
### 1. **Exploratory Data Analysis (EDA)**
- Analyzed and visualized relationships between features and target variables using scatter plots, histograms, and box plots.

### 2. **Data Preprocessing**
- Handled missing values using imputation.
- Scaled numerical features and one-hot encoded categorical features.

### 3. **Modeling**
- Trained multiple models including **Linear Regression**, **Random Forest**, and **XGBoost**.
- Tuned the **XGBoost** model using **GridSearchCV** for better performance.

### 4. **Evaluation**
- Best model: **XGBoost Regressor**.
- Performance:
  - **MSE**: 1.89
  - **R² Score**: 0.9958
  - **Cross-Validation Mean MSE**: 1.93

---
