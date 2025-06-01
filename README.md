# 📧 Spam Classification 

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

### Interpretation of the Results:

Our model demonstrates **overall strong performance**, achieving an accuracy of **92%**. This means it correctly predicted the class for 92% of the samples in our dataset.

Let's break down the metrics for each class:

#### Class 0:
* **Precision (0.92):** When the model predicted an instance as Class 0, it was correct 92% of the time. This indicates a low rate of false positives for Class 0.
* **Recall (0.95):** The model successfully identified 95% of all actual Class 0 instances. It's very good at "finding" all the Class 0 examples, resulting in few false negatives.
* **F1-score (0.93):** This balanced metric highlights the strong performance for Class 0, combining both precision and recall.
* **Support (531):** There were 531 actual instances of Class 0 in the dataset.

#### Class 1:
* **Precision (0.93):** When the model predicted an instance as Class 1, it was correct 93% of the time. This shows excellent precision for Class 1.
* **Recall (0.88):** The model correctly identified 88% of all actual Class 1 instances. While still good, it's slightly lower than Class 0's recall, suggesting a slightly higher rate of false negatives for Class 1.
* **F1-score (0.91):** The F1-score for Class 1 indicates strong performance, though marginally lower than Class 0.
* **Support (390):** There were 390 actual instances of Class 1 in the dataset.

#### Averages:
* **Macro Average:** This provides an unweighted average of the metrics across both classes. The consistent **0.92** for precision, recall, and F1-score here suggests balanced performance without being influenced by class imbalance.
* **Weighted Average:** This average considers the number of samples in each class. The results are very similar to the macro average, further confirming the model's balanced and robust performance across the dataset.

In conclusion, the model is **well-balanced** and performs consistently well across both classes, with a slight edge in recalling Class 0 instances. The high precision for both classes means that when the model makes a prediction, it's highly likely to be correct.
