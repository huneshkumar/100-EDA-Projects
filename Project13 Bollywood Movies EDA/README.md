# Project 13 — Bollywood Movies EDA

## Problem Statement

Explore Bollywood movie data to understand release patterns, genres, remakes vs originals, franchise films, cast and crew (lead star, director, music director), screen counts, and financial performance (revenue and budget in INR). The goal is to uncover trends and factors associated with box-office outcomes.

## Dataset

- **Source:** `../datasets/Bollywood_movies.csv`
- **Key columns:** Movie_Name, Release_Period, Whether_Remake, Whether_Franchise, Genre, New_Actor, New_Director, New_Music_Director, Lead_Star, Director, Music_Director, Number_of_Screens, Revenue(INR), Budget(INR)

## Analysis Performed

- Load and inspect data; shape, info, missing values.
- Analyze categorical features (genre, release period, remake/franchise flags).
- Analyze numerical features (screens, revenue, budget); ROI or profit if derived.
- Correlation and visualizations (histograms, bar charts, boxplots, heatmaps).
- Document insights on what drives revenue and budget patterns.

## Key Insights (Summary)

- Distribution of genres and release periods.
- Relationship between budget, screens, and revenue.
- Impact of remake/franchise and new talent flags on performance.

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook
