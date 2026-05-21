# Income Classification: Regularization & Ensemble Methods

**Course:** Artificial Intelligence | University of Santo Tomas
**Author:** Atasha Samantha T. Geronimo | 2DSA2

---

## Overview

Compared 10 classification models on the Adult Income dataset to predict 
whether an individual earns more than $50K/year. Models range from simple 
Linear Probability Models to regularized regression and ensemble methods — 
evaluating how regularization and complexity affect predictive performance.

## Dataset

- **Source:** UCI Adult Income Dataset (OpenML)
- **Size:** 30,162 observations × 97 features (after encoding)
- **Target:** Binary — high income (>50K) vs. low income (≤50K)
- **Class distribution:** 24.9% high-income (moderate imbalance)

## Models Compared

| Model | Accuracy | F1-Score |
|---|---|---|
| LPM (baseline) | 0.8422 | 0.6258 |
| LPM + Ridge | 0.8429 | 0.6259 |
| Logistic Regression | 0.8553 | 0.6782 |
| Logit + Ridge | 0.8556 | 0.6806 |
| Random Forest | 0.8696 | 0.7080 |
| **Gradient Boosting** | **0.8778** | **0.7285** |

## Key Findings

- Gradient Boosting was the best model overall — highest accuracy (87.78%), 
  precision (81.53%), recall (65.85%), and lowest Type II error (34.15%)
- Ridge regularization modestly improved Logistic Regression; Lasso 
  over-penalized and hurt recall significantly
- Ensemble methods outperformed all linear and regularized models, 
  capturing nonlinear relationships in income data

## Tools

`Python` `scikit-learn` `pandas` `matplotlib` `seaborn`
