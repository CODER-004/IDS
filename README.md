# Network Intrusion Detection System using Machine Learning

## Overview

This project implements a complete **Machine Learning pipeline for Network Intrusion Detection** using multiple Parquet datasets. The notebook performs data loading, preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and model saving.

The project compares **Random Forest** and **XGBoost** classifiers for multi-class network attack detection.

---

## Features

* Load multiple Parquet files
* Clean and preprocess datasets
* Create a balanced master dataset using stratified sampling
* Perform Exploratory Data Analysis (EDA)
* Encode categorical target labels
* Train-Test Split
* Data preprocessing

  * Missing value handling
  * Feature scaling
* Optional PCA for dimensionality reduction
* Optional SMOTE for handling class imbalance
* Train:

  * Random Forest
  * XGBoost
* Model evaluation using:

  * Accuracy
  * Precision
  * Recall
  * F1 Score
  * Confusion Matrix
  * Classification Report
* Feature Importance Visualization
* Save trained models and preprocessing objects

---

## Project Workflow

```text
Parquet Files
      │
      ▼
Data Cleaning
      │
      ▼
Stratified Sampling
      │
      ▼
Master Dataset Creation
      │
      ▼
Exploratory Data Analysis
      │
      ▼
Target Encoding
      │
      ▼
Train-Test Split
      │
      ▼
Preprocessing
(Standardization)
      │
      ▼
(Optional)
PCA
      │
      ▼
(Optional)
SMOTE
      │
      ▼
Train Models
├── Random Forest
└── XGBoost
      │
      ▼
Model Evaluation
      │
      ▼
Feature Importance
      │
      ▼
Save Model
```

---

## Project Structure

```
.
├── minor1.ipynb              # Complete ML pipeline
├── data/
│   ├── dataset1.parquet
│   ├── dataset2.parquet
│   └── ...
├── models/
│   ├── random_forest.pkl
│   ├── xgboost.pkl
│   ├── scaler.pkl
│   ├── encoder.pkl
│   └── pca.pkl (optional)
└── README.md
```

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* Imbalanced-learn (SMOTE)
* Matplotlib
* Seaborn

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/network-intrusion-detection.git

cd network-intrusion-detection
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Required Libraries

```text
pandas
numpy
scikit-learn
matplotlib
seaborn
xgboost
imbalanced-learn
joblib
pyarrow
```

Install them using:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn xgboost imbalanced-learn joblib pyarrow
```

---

## Dataset

Place all your **Parquet files** inside the project directory and update the `parquet_paths` list in the notebook.

Example:

```python
parquet_paths = [
    "data/file1.parquet",
    "data/file2.parquet",
    "data/file3.parquet"
]
```

---

## Models Used

### Random Forest

* Ensemble learning algorithm
* Handles nonlinear relationships
* Provides feature importance

### XGBoost

* Gradient Boosting framework
* High predictive performance
* Efficient handling of large datasets
* Regularization to reduce overfitting

---

## Evaluation Metrics

The notebook evaluates the trained models using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix
* Classification Report

---

## Outputs

The notebook generates:

* Cleaned dataset
* Master sampled dataset
* EDA summary
* Encoded labels
* Trained Random Forest model
* Trained XGBoost model
* Feature importance plots
* Saved preprocessing objects
* Saved trained models

---

## Future Improvements

* Hyperparameter tuning using GridSearchCV or Optuna
* Deep Learning models
* Explainable AI using SHAP
* Real-time intrusion detection pipeline
* Deployment using Flask/FastAPI
* Docker support

---

## Author

**Nikhil Mishra**

Final Year B.Tech CSE Student
MANIT Bhopal

---

## License

This project is intended for educational and research purposes.
