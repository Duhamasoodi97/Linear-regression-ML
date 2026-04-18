# 📈 Simple Linear Regression ML

![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![ML](https://img.shields.io/badge/Machine%20Learning-Linear%20Regression-green)
![Library](https://img.shields.io/badge/Library-Scikit--Learn-orange)

A machine learning project demonstrating a complete workflow for performing **Simple Linear Regression** using Python, Pandas, and Scikit-Learn.

---

## 📌 Overview

This project walks through the process of building a Simple Linear Regression model to predict a continuous target variable (`y`) based on a single predictor variable (`x`). The workflow covers everything from data loading and cleaning to exploratory data analysis (EDA), model training, and performance evaluation on a test dataset.

---

## ⚙️ Features

* **Data Loading & Preprocessing**: Handles missing values gracefully by dropping incomplete rows.
* **Exploratory Data Analysis (EDA)**: Includes summary statistics, missing value checks, and data distribution visualization using histograms.
* **Correlation Analysis**: Validates the relationship between variables before modeling (e.g., showing a 0.995 correlation matrix).
* **Model Training**: Implements Scikit-Learn's `LinearRegression` to find the best-fit line (Slope and Intercept).
* **Performance Evaluation**: Evaluates the model using the **R-squared ($R^2$) metric** on both training and testing datasets.
* **Visualization**: Plots predicted vs. actual values to visually verify model accuracy.

---

## 📂 Project Structure

```
Linear-Regression-ML/
│
├── train.csv                     # Training dataset (with x and y columns)
├── test.csv                      # Testing dataset (with x and y columns)
├── linear_regression.ipynb       # Main Google Colab / Jupyter notebook
└── README.md                     # Documentation
```

---

## 🚀 Getting Started

### 🔧 Prerequisites

* Python 3.7+
* Jupyter Notebook / Google Colab

### 📦 Installation

Install the required Python libraries:

```bash
pip install pandas matplotlib scikit-learn
```

---

### ▶️ Run the Project

If you are using Google Colab (as shown in the source code):
1. Upload `train.csv` and `test.csv` to your `/content/` directory.
2. Run the cells sequentially to observe the EDA and Model Evaluation.

---

## 🧠 Workflow

1. **Import Libraries**: Load `pandas`, `matplotlib.pyplot`, and `sklearn.linear_model.LinearRegression`.
2. **Load Training Data**: Read `train.csv`.
3. **Data Cleaning**: Identify missing values using `.isnull().sum()` and drop them with `.dropna()`.
4. **EDA & Visualization**: Generate histograms and a correlation matrix.
5. **Model Training**: Fit the model to find the relationship $y = mx + b$.
6. **Model Evaluation (Train)**: Calculate the $R^2$ score on the training data.
7. **Testing**: Load `test.csv`, predict $y$ using the test $x$ values, and calculate the $R^2$ score on the test data.
8. **Visualization**: Plot Actual vs Predicted values using Matplotlib.

---

## 📊 Results Summary

* **Training R-squared**: ~0.9907
* **Testing R-squared**: ~0.9888
* **Conclusion**: The model generalizes extremely well, maintaining high predictive accuracy on unseen test data.

---

## 📄 License

MIT License
