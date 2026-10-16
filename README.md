# Breast Tumor Diagnosis Classifier

An XGBoost model that classifies breast tumors as benign or malignant from 30 measurements of cell nuclei.

## Results (held-out test set, 114 samples)
- Accuracy: 96.5%
- ROC-AUC: 0.996
- Malignant precision 1.00, recall 0.90

## Approach
- Data: Wisconsin Diagnostic Breast Cancer dataset (569 samples, 30 features, no missing values)
- Prep: dropped ID and empty columns, encoded diagnosis labels, stratified 80/20 train/test split
- Model: XGBoost (200 trees, max depth 3, learning rate 0.05)
- Validation: stratified 5-fold cross-validation on the training set only

## Tools
Python, XGBoost, scikit-learn, pandas, Google Colab

## Team
Built for Catalyst at Duke with Akshay, Akari, and Connor. I worked on data preparation and the model.
