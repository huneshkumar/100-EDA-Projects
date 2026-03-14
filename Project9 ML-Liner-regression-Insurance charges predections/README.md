# Project 9 — ML: Insurance Charges Prediction

## Problem Statement

Build a **linear regression** model to predict medical insurance charges from customer attributes (age, sex, BMI, number of children, smoking status, region). The goal is to learn which factors drive cost and to produce interpretable predictions.

## Dataset

- **Source:** `../datasets/insurance.csv`
- **Key columns:** age, sex, bmi, children, smoker, region, **charges** (target)

## Analysis Performed

- Load and explore insurance data; basic EDA (shape, info, missing values).
- Encode categorical variables (sex, smoker, region) for regression.
- Split data into train/test; fit linear regression model.
- Evaluate with metrics (e.g. MAE, RMSE, R²) and residual analysis.
- Interpret coefficients and summarize insights.

## Key Insights (Summary)

- Which features most influence predicted insurance charges.
- Model performance and residual behavior.
- Practical takeaways for understanding or estimating premiums.

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Jupyter Notebook
