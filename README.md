# Fraud Detection using Machine Learning
A project for NUS DSA4263: Sense-making Case Analysis: Business and Commerce (AY2024/25 Semester 2)

## Group Members
Lee Jing Yun, Jamie

Lee Yi Hui, Joey

Liang Xiaoxin

Mei Boyu

## Project Overview
This project aims to build a fraud detection system using machine learning models on a large-scale dataset that simulates mobile money transactions. The dataset includes over 6 million records of various transaction types with a significant class imbalance between fraudulent and non-fraudulent cases. The goal is to accurately classify fraudulent transactions.

## Key Objectives
- Conduct exploratory data analysis (EDA) to uncover patterns in fraudulent behavior.
- Train and compare baseline models (Logistic Regression, Random Forest, XGBoost).
- Address severe data imbalance using techniques like scale_pos_weight and class_weight = 'balanced'.
- Engineer meaningful features (e.g. `log_amount`, `amount_z_score`, etc.) to improve signal in the dataset.
- Evaluate models using metrics such as ROC AUC, precision, recall, and F1-score.
- Compare model performance before and after feature engineering.

This project demonstrates how data science techniques can be applied to real-world financial problems and emphasizes the importance of model interpretability, feature engineering, and ethical use of data in fraud detection systems.

## Dataset

The dataset used in this project is publicly available on Kaggle:

 [Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

To use the dataset:
1. Visit the link above
2. Log in with a Kaggle account
3. Download `creditcard.csv`
4. Place it in the `data/` folder of this repository

## Project Structure

.
├── data/                    # Raw and processed datasets (excluded from GitHub if large)
├── notebooks/              # Jupyter notebooks for EDA, modeling, etc.
│   ├── 01_eda.ipynb
│   ├── 02_model_baselines.ipynb
│   ├── 03_feature_engineering.ipynb
│   └── 04_final_model_cv.ipynb
├── models/                 # Serialized models (.pkl, .joblib, etc.)
├── scripts/                # Python scripts for training, evaluation, preprocessing
├── reports/                # Visuals, final writeup, and summary charts
├── requirements.txt        # Dependencies
└── README.md

## Models Used
- Logistic Regression (Baseline)
- Decision Tree
- Random Forest
- XGBoost

## Exploratory Data Analysis (EDA)

## Feature Engineering Highlights
- `log_amount`: log-transformed transaction amount
- `amount_z_score`: standard score within each type
- `isHighAmount`: flag for high transaction amounts

  
## Handling Class Imbalance


## Model Development

## Results Summary


## How to Run
```bash
# Clone the repository
git clone https://github.com/yourusername/DSA4263.git
cd DSA4263

# Install dependencies
```bash
pip install -r requirements.txt

# Run notebook or script
jupyter notebook notebooks/03_feature_engineering.ipynb
