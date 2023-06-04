# Credit Card Fraud Detection
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

This project focuses on developing a credit card fraud detection system using machine learning techniques. The goal is to accurately identify fraudulent credit card transactions to prevent customers from being charged for unauthorized purchases.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Project Steps](#project-steps)
- [Results](#results)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Overview

In the banking industry, detecting fraudulent credit card transactions is of utmost importance to protect customers and financial institutions. This project addresses this issue by implementing machine learning models to classify transactions as either fraudulent or legitimate. The focus is on achieving high accuracy while considering precision and recall.

## Dataset

The dataset used for this project contains credit card transactions made by European cardholders in September 2013. It consists of numerical features resulting from a Principal Component Analysis (PCA) transformation, ensuring confidentiality. Key features include 'Time' (elapsed seconds since the first transaction), 'Amount' (transaction amount), and 'Class' (fraud or legitimate). The dataset is highly unbalanced, with fraudulent transactions accounting for only 0.172% of all transactions.

## Project Steps

The project follows these steps:

1. Data Preprocessing: Handle missing values, scale numerical features, and encode categorical variables.
2. Exploratory Data Analysis: Understand the distribution of features, identify patterns, and explore correlations.
3. Model Selection: Choose appropriate classification models for fraud detection, such as Logistic Regression, Decision Tree, Random Forest, K-Nearest Neighbors, and Support Vector Classifier (SVC).
4. Class Imbalance Handling: Implement undersampling techniques like Random Undersampling, Tomek Links, NearMiss, Cluster Centroids, and Condensed Nearest Neighbour to address class imbalance.
5. Model Training and Evaluation: Train the selected models on the undersampled data and evaluate their performance using metrics like accuracy and Area Under the Precision-Recall Curve (AUPRC).
6. Model Comparison: Compare the results of different models and undersampling techniques to identify the most effective combination.

## Results

The best performing model for this project is the Support Vector Classifier (SVC) when combined with the Condensed Nearest Neighbour undersampling technique. This combination achieved an AUPRC score of 0.975000, indicating its effectiveness in accurately identifying fraudulent transactions while considering precision and recall.

## Dependencies

The following dependencies are required to run the project:

- Python (version 3.10.11)
- pandas (version 1.5.3)
- scikit-learn (version 1.2.2)
- numpy (version 1.22.4)
- matplotlib (version 3.7.1)
- imblearn (version 0.10.11)
