# World Happiness Report 2024 – Analysis & Prediction

A clean, insightful exploration of the **World Happiness Report (updated 2024)** using **XGBoost** to predict **Life Ladder (happiness score)** and uncover key drivers of well-being.

---

## Overview
This project analyzes global happiness data to:
- Visualize the **distribution of happiness scores**
- Explore the **relationship between GDP and happiness**
- Build a **regression model** to predict happiness
- Reveal **feature importance** using XGBoost

---

## Dataset
- `World-happiness-report-updated_2024.csv`
- Key columns:
  - `Life Ladder` → Happiness score (0–10)
  - `Log GDP per capita`, `Social support`, `Healthy life expectancy`, etc.

---

## Key Steps

1. **Data Loading & Cleaning**
   - Handle missing values with mean imputation
2. **Exploratory Visualization**
   - Happiness distribution (histogram + KDE)
   - GDP vs Happiness (scatter plot)
3. **Modeling**
   - Train/test split (80/20)
   - **XGBoost Regressor**
4. **Feature Importance**
   - Top predictor: **Log GDP per capita** (~858)
   - Followed by **Social support**, **Generosity**, **Positive affect**

---

## Key Findings

| Insight | Details |
|-------|--------|
| **Happiness Distribution** | Near-normal, peaks at ~5/8 |
| **GDP & Happiness** | Strong positive trend, but high variance |
| **Top Driver** | **Income (Log GDP per capita)** |
| **Social Factors Matter** | Support, freedom, emotions nearly as important |
| **Least Impact** | Perceptions of corruption |

> **Income explains the most, but happiness is deeply social and emotional.**

---

## Visualizations
- Histogram: Happiness score distribution
- Scatter: GDP vs Happiness
- Bar plot: XGBoost feature importance

---

## Requirements
```txt
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
mlxtend
