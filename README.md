✈️ Flight Price Prediction — ML Pipeline (XGBoost vs Random Forest)
A clean and reproducible Machine Learning pipeline for predicting flight ticket prices using XGBoost and Random Forest.
This project benchmarks two powerful tree‑based models on a real-world Kaggle dataset and includes full preprocessing, feature engineering, model evaluation, and visualization.
📌 Project Overview
This project builds an end‑to‑end ML workflow for airfare prediction.
It includes:

Data cleaning and preprocessing

Handling numerical & categorical features

One‑Hot Encoding

Log‑transformed target regression

Training XGBoost & Random Forest models

Model evaluation using MAE, RMSE, and R²

Visual comparison of actual vs predicted prices

5‑fold cross‑validation for reliable benchmarking

Dataset source:
https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction

🧠 Models Used
XGBoost Regressor
500 estimators

Learning rate: 0.05

Max depth: 8

Subsample & colsample tuning

Wrapped with TransformedTargetRegressor for log‑target regression

Random Forest Regressor
200 trees

Bootstrap aggregation

Also wrapped with log‑target regression for fair comparison

🛠️ Tech Stack
Python

NumPy / Pandas

Scikit‑Learn

XGBoost

Matplotlib

ColumnTransformer + Pipeline API

📊 Evaluation Metrics
Each model is evaluated using:

MAE — Mean Absolute Error

RMSE — Root Mean Squared Error

R² Score

5‑Fold Cross‑Validation

A plot comparing the first 100 predictions is also included.

📁 Project Structure

├── data/

│   └── Clean_Dataset.csv

├── notebooks/

│   └── model_training.ipynb

├── src/

│   ├── preprocessing.py

│   ├── train_xgb.py

│   ├── train_rf.py

│   └── evaluate.py

├── README.md

└── requirements.txt

📈 Results Summary
XGBoost generally performs better on RMSE and R²

Random Forest provides stable baseline performance

Log‑target regression significantly improves both models
