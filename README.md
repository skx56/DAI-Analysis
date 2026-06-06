# Restaurant Tip Prediction and Regression Analysis

This repository contains an end-to-end machine learning pipeline designed to analyze restaurant tipping behavior and predict tip amounts based on various customer and dining attributes. Using the popular `tips` dataset, the project walks through data preprocessing, exploratory data analysis (EDA), statistical diagnostic testing, and the benchmarking of multiple regression algorithms to identify the most accurate predictive model.

---

## **Key Features and Workflow**

* **Data Preprocessing:** Cleans and formats the data by mapping categorical variables (e.g., Sex, Smoker status, Meal time) into machine-readable numerical formats using encoding techniques.
* **Exploratory Data Analysis (EDA):** Leverages `seaborn` and `matplotlib` to visualize relationships within the data. This includes pair plots for variable distributions, correlation heatmaps to identify multicollinearity, and box plots analyzing tip amounts across different days of the week.
* **Statistical Diagnostics:** * Performs the **Linear Rainbow Test** via `statsmodels` to check the underlying assumption of linearity in the dataset.
* Generates a **Residuals Plot** (fitted values vs. residuals) with a LOWESS smoothing line to visually assess homoscedasticity and model fit for standard linear regression.


* **Model Benchmarking:** Splits the data into training and testing sets (80/20) and evaluates seven different machine learning regression models:
* Linear Regression
* Ridge Regression
* Lasso Regression
* Decision Tree Regressor
* Random Forest Regressor
* Support Vector Regressor (SVR)
* K-Nearest Neighbors (KNN) Regressor


* **Performance Evaluation:** Compares models based on standard regression metrics: **R² Score**, Mean Absolute Error (**MAE**), and Mean Squared Error (**MSE**).
* **Feature Importance Analysis:** Utilizes a Random Forest Regressor to extract, rank, and plot the relative importance of each feature in predicting the final tip amount.

---

## **Key Findings**

Based on the evaluation metrics, **Support Vector Regression (SVR)** with an RBF kernel outperformed the other algorithms, achieving the highest R² Score (~0.569) and the lowest Mean Absolute Error (~0.570) for this specific dataset.

---

## **Technologies & Libraries Used**

* **Data Manipulation:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`
* **Machine Learning:** `scikit-learn`
* **Statistical Modeling:** `statsmodels`
