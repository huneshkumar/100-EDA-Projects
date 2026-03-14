# Project 10 — ML: Ford Car Price Prediction

## Problem Statement

Build a **linear regression** model to predict Ford car prices using features such as model, year, mileage, transmission, fuel type, tax, mpg, and engine size. The goal is to identify which factors drive price and to produce interpretable predictions for used Ford vehicles.

## Dataset

- **Source:** `../datasets/ford.csv`
- **Rows:** 17,966 used Ford car listings
- **Key columns:**
  - **model** — Ford model name (e.g. Fiesta, Focus)
  - **year** — Production year
  - **price** — Target; price in $
  - **transmission** — Automatic, Manual, Semi-Auto
  - **mileage** — Miles traveled
  - **fuelType** — Petrol, Diesel, Hybrid, Electric, Other
  - **tax** — Annual tax
  - **mpg** — Miles per gallon
  - **engineSize** — Engine size

## Analysis Performed

- Load and explore Ford used-car data; shape, info, describe, missing values.
- EDA: value counts (model), distributions, and visualizations.
- Encode categorical variables: one-hot encoding (`get_dummies`) for model, fuelType, transmission (with `drop_first=True` to avoid multicollinearity).
- Scale numerical features using `StandardScaler`.
- Split data into train/test (e.g. 80/20); fit **LinearRegression** from scikit-learn.
- Evaluate with metrics (e.g. MAE, RMSE, R²) and interpret coefficients.
- Optional: compare with label-encoded version of categoricals.

## Key Insights (Summary)

- Which features (year, mileage, engine size, model, transmission, fuel type) most influence predicted price.
- Model performance on test set and residual behavior.
- Practical takeaways for pricing or buying used Ford cars.

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn (LinearRegression, train_test_split, StandardScaler), Jupyter Notebook
