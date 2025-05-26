# 📧 Spam Classification Using Bernoulli Distribution

This project analyzes the UCI Spambase dataset using the **Bernoulli distribution** to model the binary classification of emails as spam (`1`) or not spam (`0`). It demonstrates how probabilistic thinking, statistical modeling, and machine learning can be combined to build interpretable solutions to real-world problems.

---

## 📌 Project Overview

- ✅ Fetches and explores the [Spambase dataset](https://archive.ics.uci.edu/dataset/94/spambase) using the `ucimlrepo` Python package.
- ✅ Estimates the **empirical probability** of spam using the Bernoulli distribution.
- ✅ Simulates spam labels with `scipy.stats.bernoulli`.
- ✅ Visualizes both actual and simulated distributions.
- ✅ Trains a **Logistic Regression** model for binary classification.
- ✅ Evaluates the model with accuracy and classification metrics.

---

### 🎯 Bernoulli Distribution
The Bernoulli distribution is used to model the probability of a binary outcome (success/failure). In this project, the outcome is:
- `1` → Spam email
- `0` → Not Spam email

### 📊 Logistic Regression
A probabilistic classification algorithm used to model the relationship between input features and a binary target.

---

## 📁 Files

- `bernoulli_spam_analysis.ipynb`: Main notebook with code and visualizations.
- `README.md`: Project overview and documentation.

---

## 🛠️ Tools & Libraries

- `Python 3.10+`
- `Pandas`
- `Seaborn`, `Matplotlib` for visualizations
- `Scikit-Learn` for modeling
- `Scipy` for statistical simulation
- `ucimlrepo` to fetch datasets directly from UCI

---

## 📉 Results

- Estimated probability of an email being spam (from data): **~13-14%**
- Clear binary separation between spam and non-spam emails
- Logistic Regression achieved strong performance on test data:
  - **Precision**, **Recall**, and **F1 Score** well balanced for both classes

