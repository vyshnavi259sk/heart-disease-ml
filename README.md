# Heart Disease Prediction — End-to-End Machine Learning Pipeline

## Overview
End-to-end machine learning project predicting heart disease using
the Heart Failure Prediction dataset (918 patients, 12 features).
Covers the full ML pipeline from EDA through to deep learning.

## Techniques Covered
| Topic | Method |
|---|---|
| Unsupervised Learning | K-Means, Hierarchical Clustering |
| Regression | Linear Regression (Age → MaxHR) |
| Classification | Logistic Regression, KNN, Decision Tree |
| Ensemble Methods | Random Forest, Gradient Boosting |
| Probabilistic | Naive Bayes |
| Deep Learning | MLP Neural Network |
| Evaluation | 5-Fold CV, Paired t-test, Confusion Matrix |

## Results
5-fold CV accuracy, with all preprocessing (scaling, feature selection) and
hyperparameter search (K, depth, grid search) fit inside the training folds
only — no test-set or full-dataset leakage into any model's selection.

| Model | CV Accuracy |
|---|---|
| Random Forest | **86.5%** ← Winner |
| Logistic Regression | 85.8% |
| Gradient Boosting | 85.6% |
| KNN (K=29) | 84.9% |
| Decision Tree | 84.7% |
| Naive Bayes | 84.0% |
| Neural Network | 83.0% |

## Key Findings
- Random Forest has the best mean CV accuracy, but a paired t-test shows it's
  only *statistically* significant against the Neural Network (p < 0.05) —
  it is not significantly better than Logistic Regression, KNN, Decision
  Tree, Gradient Boosting, or Naive Bayes once everything is tuned fairly
- ST_Slope, ChestPainType, and MaxHR are the strongest predictors
- Neural networks underperform on small tabular datasets
- Cross-validation gives more reliable estimates than a single test split

## Dataset
[Heart Failure Prediction — Kaggle](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)

## Author
Vyshnavi Sunil Kumar
