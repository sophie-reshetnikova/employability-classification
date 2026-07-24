# Graduate Employability Prediction

## Overview

This project applies machine learning classification techniques to predict graduate employability outcomes. The aim is to compare different classification models and identify factors associated with successful employment.

## Dataset

The dataset used in this project was obtained from Kaggle:

[Student Employability Dataset](https://www.kaggle.com/datasets/likithagedipudi/campus-placement-prediction)
The dataset contains information about student academic performance, skills, experience, and other employability-related factors. The target variable is:

- `placed = 1`: student successfully placed/employed
- `placed = 0`: student not placed/employed

The dataset is imbalanced, with the majority of observations belonging to the positive employment outcome.

## Methodology

The following steps were performed:

- Data preprocessing and feature transformation
- Feature engineering
- Train-test splitting
- 5-fold cross-validation
- Classification model comparison
- Hyperparameter tuning using GridSearchCV

## Models

Three classification algorithms were evaluated:

- Logistic Regression
- Support Vector Machine (SVM)
- K-Nearest Neighbours (KNN)

## Model Evaluation

Due to class imbalance, accuracy was not considered an appropriate evaluation metric. Models were compared using precision, recall, and F1-score, with particular focus on the minority class (`placed = 0`).

The final model was selected based on cross-validated F1-score performance for the minority class.

## Results

Logistic Regression achieved the strongest overall performance among the evaluated models. Hyperparameter tuning was applied to improve performance, and model coefficients were analysed to identify influential predictors of employment outcomes.

Key factors associated with employment likelihood included:

- Academic performance
- Skill-related factors
- Work experience

The number of academic backlogs showed a negative relationship with employment outcomes.

## Technologies Used

- Python
- Jupyter Notebook
- pandas
- NumPy
- scikit-learn
- matplotlib

## Author

Sophie Reshetnikova
