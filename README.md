# Predicting Weight Using Machine Learning

## Overview
This project uses machine learning to predict a person’s weight based on various features like height, BMI, calories burned, and workout type. The model is trained using **XGBoost** and tuned with **GridSearchCV** for optimal performance. This project showcases the power of machine learning in real-world prediction tasks.

---
## How to Run the Project

### 1. **Clone the Repository**
```bash
git clone https://github.com/ivykogo/Weight_prediction-model.git
```
## Dataset
The dataset contains **973 rows** and **15 columns** with data on individuals' physical attributes and workout habits.

- **Features**:
  - **Height (m)**
  - **Calories Burned**
  - **Fat Percentage**
  - **BMI**
  - **Gender**
  - **Workout Type**
  - **Session Duration (hours)**

- **Target**: **Weight (kg)**

---

## Steps

### 1. **Exploratory Data Analysis (EDA)**
- Analyzed relationships between features and target variable.
  - Visualized distributions with **scatter plots**, **histograms**, and **box plots**.
  - Examined how features like **BMI**, **Height**, and **Calories Burned** relate to **Weight (kg)**.

### 2. **Data Preprocessing**
- Handled missing data using **SimpleImputer** (mean imputation for numeric features, most frequent for categorical).
- Scaled numeric features using **StandardScaler**.
- One-hot encoded categorical features (**Gender**, **Workout Type**).

### 3. **Modeling**
- Trained multiple models to predict weight:
  - **Linear Regression**: Baseline model.
  - **Random Forest Regressor**: Captured non-linear relationships.
  - **XGBoost Regressor**: Best-performing model, optimized using **GridSearchCV** for tuning parameters like **learning rate**, **max depth**, and **n_estimators**.

### 4. **Evaluation**
- **Best Model**: **XGBoost Regressor**
  - **MSE**: 1.89 (Mean Squared Error)
  - **R² Score**: 0.9958 (99.58% explained variance)
  - **Cross-Validation MSE**: 1.93

---

