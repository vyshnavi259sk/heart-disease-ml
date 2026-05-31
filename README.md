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
| Model | CV Accuracy |
|---|---|
| Random Forest | **86.6%** ← Winner |
| Logistic Regression | 85.8% |
| Gradient Boosting | 85.1% |
| Decision Tree | 84.7% |
| Naive Bayes | 84.0% |
| KNN (K=8) | 83.4% |
| Neural Network | 81.7% |

## Key Findings
- Random Forest statistically outperforms KNN, Decision Tree and Neural Network (p < 0.05)
- ST_Slope, ChestPainType, and MaxHR are the strongest predictors
- Neural networks underperform on small tabular datasets
- Cross-validation gives more reliable estimates than a single test split

## Dataset
[Heart Failure Prediction — Kaggle](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)

## Author
Vyshnavi Sunil Kumar
