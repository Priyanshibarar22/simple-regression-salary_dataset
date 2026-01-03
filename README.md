# Simple Linear Regression – Salary vs Experience

This project implements a **simple** Linear Regression model to predict an employee's salary based on their years of experience.It uses the classic `Salary_Data.csv` dataset and demonstrates the end‑to‑end machine learning workflow: data loading, train‑test split, model training, prediction, and visualization.

## Project Overview

- Problem: Predict salary from years of experience (one feature, one target).
- Algorithm: Simple Linear Regression from scikit‑learn.
- Language: Python
- Libraries: `numpy`, `pandas`, `matplotlib`, `scikit-learn`.

## Dataset

- File: `Salary_Data.csv`.
- Columns:
  - `YearsExperience`: Numeric, years of work experience.
  - `Salary`: Numeric, annual salary.

The dataset is loaded using pandas:

```python
dataset = pd.read_csv('Salary_Data.csv')
X = dataset.iloc[:, :-1].values
y = dataset.iloc[:, -1].values

