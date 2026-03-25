# Project 15 — Kentucky Real Estate (EDA + ML Prep)

## Problem Statement

Analyze Kentucky real estate listings and prepare a **clean, encoded feature matrix** to predict **list price** (`listPrice`). The notebook combines exploratory analysis, data cleaning, feature engineering, and scaling so you can plug in a regression model in the next cells.

## Dataset

- **Source:** `../datasets/kentucky_real_estate.csv`
- **Scale:** ~8,500 listings (12 raw columns before cleaning)
- **Key columns:** type, sub_type, text, listPrice, sqft, stories, beds, baths, baths_full, baths_full_calc, garage, year_built

## Analysis Performed

1. **EDA** — Shape, `info`, `describe`, missing values, group-by plots (e.g. price by type, garage counts).
2. **Data cleaning** — Drop duplicate rows; impute numerics with **median** and categoricals with `"Unknown"`; drop high-cardinality / leaky columns (`text`, `sub_type`, `baths_full_calc`) as in the notebook.
3. **Feature engineering** — Bin `listPrice` into **price tiers** (`category`); one-hot encode **`type`** and **`category`**; derive **`house_age`** from `year_built` (reference year in notebook); drop raw `year_built` where applicable.
4. **Scaling** — `StandardScaler` on selected numeric features (dummy columns excluded from scaling per notebook comments).
5. **Modeling setup** — Build **`X`** (all features except `listPrice`) and **`Y`** = `listPrice` for regression (train/test split and estimator can be added after).

## Key Insights (Summary)

- Typical price, sqft, and bedroom/bathroom distributions; outliers in garage / extreme prices.
- Missingness patterns (e.g. `sub_type`, `garage`, `year_built`).
- How property **type** and **price tier** relate to list price before encoding.

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn (`StandardScaler`), Jupyter Notebook
