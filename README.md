# Predict Calorie Expenditure 🤵

This repository contains our solution for the Kaggle competition: **Playground Series - Season 5, Episode 5 (S5E5)**, where the goal is to predict **calorie expenditure** based on various physiological and biometric features.

## Background 🧠

In an era where fitness and health monitoring have become increasingly digitized, estimating calorie expenditure accurately is critical. Whether it's for wearables, health tracking apps, or personal fitness goals, having a model that can predict how much energy is burned during physical activities can help users and systems make better health decisions.
This challenge provides a rich dataset simulating real-world biometric and physical activity data. The goal is to build a regression model that predicts the amount of calories burned during an exercise session, based on personal and session-related features.

## Objective 🎯

Develop and evaluate machine learning models that predict the number of calories expended during physical activity.

---

## 📂 Dataset Overview

The dataset consists of:

- `train.csv`: Training data with 7500+ observations.
- `test.csv`: Test data without the target column.
- `sample_submission.csv`: Template for predictions.

### 📊 Features:

- `age`: Age of the individual (years)
- `height`: Height (cm)
- `weight`: Weight (kg)
- `duration`: Duration of exercise (minutes)
- `heart_rate`: Average heart rate during the session
- `body_temp`: Average body temperature (Celsius)

### 🎯 Target:
- `calories`: Total energy expenditure during the exercise session (kcal)

---

## 🧪 Approach

1. **EDA & Preprocessing**
   - Checked for null values, distributions, correlations, and outliers.
   - Normalized features where appropriate.
   - Explored log transforms and feature interactions.

2. **Model Training**
   - Tried multiple regression models:
     - Linear Regression
     - Random Forest Regressor
     - Gradient Boosting Regressor
     - XGBoost Regressor
     - CatBoost Regressor
   - Hyperparameter tuning using GridSearchCV and Optuna

3. **Evaluation Metrics**
   - Mean Absolute Error (MAE) – Primary metric for Kaggle leaderboard.
   - Root Mean Squared Error (RMSE)
   - R² Score

---
