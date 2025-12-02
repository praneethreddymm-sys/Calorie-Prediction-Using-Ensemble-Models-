# Calorie-Prediction-Using-Ensemble-Models-
 Developed a calorie prediction model using Linear Regression, Random Forest, XGBoost, and CatBoost, based on various influencing factors. Applied feature scaling and evaluation metrics (MAE, MSE, R²) to ensure accurate and reliable predictions.people being cared for; having numerous children will raise the costs associated with health care for the entire family. 
 <h1 align="center">Calorie Prediction Using Regression Techniques</h1>

<div align="center">
  <h4>A Comparative Analysis of ML Regression Models for Calorie Burn Prediction</h4>
</div>

---

## 📌 Overview

This project predicts the **calories burned** by an individual during physical exercise using multiple machine learning regression algorithms.  
The goal is to compare different regression techniques and determine the most effective model.

The models evaluated:

- **Multiple Linear Regression**
- **Random Forest Regression**
- **XGBoost Regression**
- **CatBoost Regression**

Performance is measured using:

- **MAE** (Mean Absolute Error)  
- **MSE** (Mean Squared Error)  
- **R² Score**

---

## 📂 Dataset Description

Two datasets from **Kaggle** are used:

### **1. `calories.csv`**
Contains:  
- `User_ID`  
- `Calories` (target variable)

### **2. `exercise.csv`**
Contains:  
- `User_ID`  
- `Gender`  
- `Age`  
- `Height`  
- `Weight`  
- `Duration` of exercise  
- `Body Temperature`  
- `Heart Rate`  

Both datasets are **merged on `User_ID`** to create a unified dataset.

---

## 🧹 Data Preprocessing

Preprocessing steps:

- Dropping non-informative column: **`User_ID`**
- Handling missing values:
  - Numerical → **mean**
  - Categorical → **mode**
- Encoding categorical feature:
  - `Gender` → numerical encoding
- Merging datasets into a single training file

---

## 🧠 Features Used

| Feature | Type | Description |
|--------|------|-------------|
| Gender | Categorical | Male/Female |
| Age | Numerical | Age of person |
| Height | Numerical | Height (cm) |
| Weight | Numerical | Weight (kg) |
| Duration | Numerical | Exercise duration (min) |
| Body Temperature | Numerical | Temp during exercise |
| Heart Rate | Numerical | Heartbeat during activity |

🎯 **Target variable:**  
✔ `Calories`

---

## 🔧 Methodology

### 1️⃣ Dataset Acquisition  
Load both datasets and merge using `User_ID`.

### 2️⃣ Preprocessing  
Cleaning, encoding categorical features, handling missing data.

### 3️⃣ Model Selection  
We trained the following regression algorithms:

- **Multiple Linear Regression**  
- **Random Forest Regression**  
- **XGBoost Regression**  
- **CatBoost Regression**

### 4️⃣ Train-Test Split  
Dataset split into:

- **80% Training data**
- **20% Testing data**

### 5️⃣ Model Training  
Each model is trained on the training set and evaluated on the test set.

---

## 📊 Performance Metrics

| Model | MSE | MAE | R² Score |
|--------|--------|--------|--------|
| **Multiple Linear Regression** | 514.00 | 18.00 | 0.8724 |
| **Random Forest Regression** | 268.28 | 12.88 | 0.9034 |
| **XGBoost Regression** | 220.80 | 10.19 | 0.9403 |
| **CatBoost Regression** | 200.90 | 9.89 | **0.9779** |

✔ **CatBoost is the best performing model.**  
❌ **Multiple Linear Regression performs the worst.**

---

## 📈 Visualizations
![image]()

 
