# Fraud Detection Using Machine Learning

## Overview
This project focuses on detecting fraudulent transactions using machine learning techniques. The dataset used is a credit card transaction dataset containing transformed features. The main goal is to preprocess the data, explore patterns, handle class imbalance, and train models to effectively identify fraud.

## Approach

### 1️⃣ Data Understanding & Preprocessing
- Load the dataset and check for missing values.
- The features V1 to V28 are transformed using PCA, so no additional feature engineering is required.
- Scale the `Amount` and `Time` features using `StandardScaler` to normalize the values.
- Handle class imbalance as fraud cases are rare.


