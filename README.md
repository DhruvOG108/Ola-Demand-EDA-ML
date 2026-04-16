# 🚕 Ola Ride Demand Forecasting using Machine Learning

## 📌 Overview

This project focuses on predicting hourly ride requests for an Ola-like bike service using Machine Learning. The goal is to understand demand patterns and build models that can forecast ride requests based on time, weather, and seasonal features.

---

## 📂 Dataset

The dataset contains information such as:

* Date & time of request
* Season and weather conditions
* Number of casual and registered users
* Total ride count (target variable)

---

## ⚙️ Tech Stack

* Python
* NumPy & Pandas
* Matplotlib & Seaborn
* Scikit-learn
* Jupyter Notebook

---

## 🔍 Project Workflow

### 1. Data Preprocessing

* Converted datetime column into:

  * Year, Month, Day, Hour
* Created new features:

  * Weekday/Weekend
  * AM/PM
  * Holiday indicator

---

### 2. Exploratory Data Analysis (EDA)

* Analyzed ride demand across:

  * Time of day
  * Months
  * Weather conditions
* Visualized distributions and detected outliers

---

### 3. Feature Engineering

* Removed irrelevant columns
* Handled outliers in:

  * Wind speed
  * Humidity
* Avoided data leakage by removing highly correlated features

---

### 4. Model Training

Models used:

* Linear Regression
* Lasso Regression
* Ridge Regression
* Random Forest Regressor

---

### 5. Evaluation

* Metric used: Mean Absolute Error (MAE)
* Compared training vs validation performance
* Identified overfitting in Random Forest

---

## 📊 Results

* Linear models performed consistently
* Random Forest showed slight overfitting
* Demand is highly influenced by:

  * Time of day
  * Season
  * Holidays

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone <your-repo-link>
cd ola-ride-forecast
```

### 2. Create environment

```bash
conda create -n ola-ml python=3.10
conda activate ola-ml
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run Jupyter Notebook

```bash
jupyter notebook
```

---

## 📌 Future Improvements

* Hyperparameter tuning
* Use XGBoost for better accuracy
* Deploy model using Streamlit or Flask
* Add real-time prediction capability

---
