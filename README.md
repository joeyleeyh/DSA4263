# DSA4263 Final Project - Fraud Detection using Machine Learning

## Project Overview
This project aims to build a fraud detection model using the Paysim dataset which simulates mobile money transactions. The goal is to accurately classify fraudulent transactions.

## Key Objectives
- Explore and understand the dataset via EDA
- Address data imbalance using techniques like scale_pos_weight and class_weight = 'balanced'
- Engineer meaningful features (e.g. `log_amount`, `amount_z_score`, etc.)
- Train and evaluate models (Random Forest, XGBoost, etc.)
- Compare model performance before and after feature engineering

## Project Structure

## Models Used
- Logistic Regression (Baseline)
- Decision Tree
- Random Forest
- XGBoost

## Feature Engineering Highlights
- `log_amount`: log-transformed transaction amount
- `amount_z_score`: standard score within each type
- `isHighAmount`: flag for high transaction amounts

## Results Summary
- Best Model: **XGBoost**
- AUC Score: `0.97+` after tuning and class balancing
- Improved recall for fraud cases using SMOTE

## How to Run
```bash
# Clone the repository
git clone https://github.com/yourusername/DSA4263.git
cd DSA4263

# Install dependencies
pip install -r requirements.txt

# Run notebook or script
jupyter notebook notebooks/03_feature_engineering.ipynb
