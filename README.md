# 🌧️ Rainfall Prediction Classifier - Australia Weather

This project is a supervised machine learning classification task that predicts **whether it will rain tomorrow** in different regions of Australia, based on weather data from the previous day.

> 📁 Notebook: `AUSWeather.ipynb`

---

## 📌 Problem Statement

Given daily weather observations (e.g., temperature, humidity, wind speed) across various Australian locations, the goal is to predict the binary outcome:  
**RainTomorrow**: `Yes` or `No`.

This helps with weather forecasting, agricultural planning, and flood prevention.

---

## 🗃️ Dataset

- **Source**: [Kaggle - Rain in Australia](https://www.kaggle.com/jsphyg/weather-dataset-rattle-package)
- **Size**: ~142,000 records with 24 features
- **Features Include**:
  - `Location`, `Date`
  - `MinTemp`, `MaxTemp`, `Rainfall`
  - `WindGustSpeed`, `Humidity9am`, `Pressure9am`, etc.
  - Target: `RainTomorrow`

---

## ⚙️ Project Pipeline

1. **Data Cleaning**
   - Handling missing values
   - Dropping or imputing nulls
   - Encoding categorical variables

2. **Exploratory Data Analysis (EDA)**
   - Correlation heatmaps
   - Rain distribution by region and season

3. **Feature Engineering**
   - Label encoding
   - Binary classification target

4. **Modeling**
   - Algorithms used:
     - Logistic Regression
     - Random Forest Classifier
     - XGBoost
   - Evaluation Metrics:
     - Accuracy, Precision, Recall, F1 Score
     - Confusion Matrix

5. **Model Comparison**
   - Model performance plotted and compared
   - Best model selection based on F1-score and ROC-AUC

---

## 📊 Results

- Random Forest and XGBoost performed best.
- F1-Score of ~0.85 achieved on test set.
- Important features: `Humidity3pm`, `RainToday`, `Rainfall`, and `Pressure9am`.

---

## 📦 Requirements

You can run this project in a Jupyter notebook environment.

Install dependencies via:

```bash
pip install -r requirements.txt
