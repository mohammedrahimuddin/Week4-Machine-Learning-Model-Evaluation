# Week 4 - Machine Learning Model Development and Evaluation

## Project Title
Titanic Survival Prediction Using Logistic Regression

## Project Overview
This project focuses on developing and evaluating a machine learning classification model using the Titanic dataset. The objective is to predict whether a passenger survived based on features such as passenger class, gender, age, family information, fare, and port of embarkation.

Logistic Regression was selected as the classification algorithm because it is simple, interpretable, and suitable for binary classification problems.

## Objectives
- Prepare and clean the Titanic dataset
- Select relevant features for prediction
- Encode categorical variables
- Split the dataset into training and testing sets
- Train a Logistic Regression model
- Evaluate model performance using multiple metrics
- Analyze the confusion matrix and ROC curve
- Understand feature importance through model coefficients

## Dataset
- Rows: 891
- Target Variable: `Survived`
- Target Classes:
  - 0 = Did Not Survive
  - 1 = Survived

### Selected Features
- Pclass
- Sex
- Age
- SibSp
- Parch
- Fare
- Embarked

## Machine Learning Model

**Algorithm:** Logistic Regression

**Train-Test Split:** 80% Training / 20% Testing

**Random State:** 42

## Model Performance

| Metric | Score |
|---|---:|
| Accuracy | 80.45% |
| Precision | 79.31% |
| Recall | 66.67% |
| F1-Score | 72.44% |
| ROC-AUC | 84.43% |

## Confusion Matrix

The model correctly predicted:
- 98 passengers who did not survive
- 46 passengers who survived

It incorrectly predicted:
- 12 false positives
- 23 false negatives

## Project Structure

```text
Week4_Machine_Learning/
│
├── notebooks/
│   └── titanic_ml_model.ipynb
│
├── report/
│   ├── final_report_week04.docx
│   └── model_evaluation_results.csv
│
├── visualizations/
│   ├── confusion_matrix.png
│   ├── feature_importance.png
│   └── roc_curve.png
│
└── .gitignore
