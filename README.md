# Fraud Detection Using Machine Learning

## Overview
This project focuses on detecting fraudulent transactions using machine learning techniques. The dataset used is a credit card transaction dataset containing transformed features. The main goal is to preprocess the data, explore patterns, handle class imbalance, and train models to effectively identify fraud.

## Approach

### 1️⃣ Data Understanding & Preprocessing
- Load the dataset and check for missing values.
- The features V1 to V28 are transformed using PCA, so no additional feature engineering is required.
- Scale the `Amount` and `Time` features using `StandardScaler` to normalize the values.
- Handle class imbalance as fraud cases are rare.

### 2️⃣ Exploratory Data Analysis (EDA)
- Visualize distributions of `Amount` and `Time` using histograms.
- Compute and visualize the correlation matrix between features.
- Compare fraud vs. non-fraud transactions using boxplots and histograms.

### 3️⃣ Feature Selection
- Remove irrelevant or highly correlated features (if needed).
- Use feature importance techniques like Random Forest or Mutual Information.

### 4️⃣ Handling Imbalanced Data
- Use techniques such as:
  - **Undersampling**: Reduce the number of non-fraud cases.
  - **Oversampling**: Generate synthetic fraud cases using SMOTE.

### 5️⃣ Model Selection & Training
Train multiple machine learning models and compare performance:
- **Logistic Regression** - A simple and interpretable model.
- **Random Forest** - Works well with imbalanced data.
- **XGBoost** - Highly effective for fraud detection.
- **Anomaly Detection Models** - Like Isolation Forest for identifying outliers.

### 6️⃣ Model Evaluation
Since fraud detection is an imbalanced classification problem, we use:
- **Precision & Recall** - To minimize false negatives and detect fraud accurately.
- **F1-score** - A balance between precision and recall.
- **AUC-PR (Area Under Precision-Recall Curve)** - The best metric for fraud detection models.

## Dependencies
- Python 3.x
- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `scikit-learn`, `xgboost`, `imbalanced-learn`

## Usage
1. Clone the repository:
   ```sh
   git clone https://github.com/AmanRai264/fraud-detection.git
   cd fraud-detection
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the preprocessing and model training scripts:
   ```sh
   python train_model.py
   ```

## Results
The model's performance is evaluated using precision, recall, F1-score, and AUC-PR to ensure accurate fraud detection. The best-performing model is selected based on these metrics.

## Future Improvements
- Implement deep learning techniques for fraud detection.
- Experiment with additional anomaly detection algorithms.

## Author
**Aman Rai** - Aspiring Data Analyst | Machine Learning Enthusiast


