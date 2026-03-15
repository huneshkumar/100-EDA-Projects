# Project 11 — ML: House Price Prediction

## Problem Statement

Build a **linear regression** model to predict median house prices (MEDV) using the Boston Housing dataset. Features include crime rate, lot size, industry, river boundary, NOX, average rooms, age, distances, radial highways, tax, pupil–teacher ratio, and demographic metrics. The goal is to identify which factors drive price and to produce interpretable predictions.

## Dataset

- **Source:** Loaded via **OpenML** in the notebook (`fetch_openml`), not a local CSV.
- **Key columns:** CRIM, ZN, INDUS, CHAS, NOX, RM, AGE, DIS, RAD, TAX, PTRATIO, B, LSTAT, **MEDV** (target — median value in $1000s).

## Analysis Performed

- Load Boston Housing data with scikit-learn / OpenML; explore shape, info, describe.
- EDA and visualizations; handle any missing or encoded values.
- Prepare features (X) and target (y); train/test split.
- Fit **LinearRegression**; evaluate with R², MAE, RMSE; interpret coefficients.

## Key Insights (Summary)

- Which features most influence predicted house price (e.g. RM, LSTAT).
- Model performance and residual behavior.
- Practical takeaways for understanding housing prices.

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn (LinearRegression, fetch_openml), Jupyter Notebook
