# Credit Card Fraud Detection using Supervised Machine Learning

## Project Overview

This project was completed as part of the **DecodeLabs Data Science Internship**. The objective was to build and evaluate supervised machine learning models capable of detecting fraudulent credit card transactions.

Credit card fraud detection is a challenging classification problem because fraudulent transactions represent only a very small percentage of all transactions. To address this class imbalance, **SMOTE (Synthetic Minority Oversampling Technique)** was applied before training the models.

---

## Project Objectives

* Perform exploratory data analysis (EDA) on the credit card transaction dataset.
* Preprocess and prepare the data for machine learning.
* Handle class imbalance using SMOTE.
* Train and compare multiple supervised learning models.
* Optimize model performance through hyperparameter tuning.
* Evaluate models using metrics suitable for imbalanced datasets.

---

## Dataset

The project uses the **Credit Card Fraud Detection** dataset containing anonymized credit card transactions.

**Features include:**

* Time
* V1–V28 (anonymized features obtained using PCA)
* Amount
* Class (Target Variable)

  * **0** → Legitimate Transaction
  * **1** → Fraudulent Transaction

> **Note:** The original dataset is not included in this repository because of its size. You can download it from the original source:
>
> **Dataset Link:** [(https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)]

---

## Project Workflow

### 1. Exploratory Data Analysis (EDA)

* Explored the dataset structure and class distribution.
* Identified the severe class imbalance between fraudulent and legitimate transactions.
* Visualized important patterns and relationships in the data.

### 2. Data Preprocessing

* Checked for missing values and data consistency.
* Prepared the dataset for model training.
* Applied feature scaling where appropriate.

### 3. Handling Class Imbalance

* Applied **SMOTE (Synthetic Minority Oversampling Technique)** to balance the training dataset.
* Improved the model's ability to identify fraudulent transactions.

### 4. Model Training

The following supervised learning algorithms were implemented:

* Logistic Regression
* Random Forest Classifier

### 5. Hyperparameter Tuning

Hyperparameter tuning was performed on the Random Forest model to improve predictive performance and select the optimal model configuration.

### 6. Model Evaluation

Since fraud detection is an imbalanced classification problem, the models were evaluated using:

* Precision
* Recall
* ROC-AUC Score

These metrics provide a more meaningful evaluation than accuracy for highly imbalanced datasets.

---

## Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* imbalanced-learn (SMOTE)

---

## Repository Contents

* `Project2_Fraud_Detection.ipynb` – Complete project notebook
* `README.md` – Project documentation

---

## Results

* Successfully built an end-to-end fraud detection pipeline.
* Addressed class imbalance using SMOTE.
* Compared Logistic Regression and Random Forest models.
* Improved Random Forest performance through hyperparameter tuning.
* Selected the tuned Random Forest model based on its evaluation metrics.

---

## Conclusion

This project demonstrates a complete supervised machine learning workflow for fraud detection, including data preprocessing, handling imbalanced data, model training, hyperparameter tuning, and evaluation.

By focusing on **Precision**, **Recall**, and **ROC-AUC** instead of accuracy, the project provides a more reliable approach for detecting fraudulent credit card transactions in highly imbalanced datasets.
