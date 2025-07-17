# Parkinso's-Disease-Prediction
## Project Description
This project aims to predict the presence of Parkinson's disease using voice measurements. The project involves loading and preprocessing the dataset, handling class imbalance, training various classification models, and evaluating their performance.

## Methodology
### Data Loading and Exploration: 
The parkinson_disease.csv dataset was loaded and inspected for its structure, data types, and missing values.
### Data Preprocessing:
Data was grouped by 'id' to get the mean of features for each individual.
Highly correlated features (correlation > 0.7) were removed.
The top 30 features were selected using the Chi-squared test after normalizing the features using MinMaxScaler.
### Data Balancing: 
The dataset was balanced using Random Over-Sampling to address the class imbalance in the target variable.
### Model Training: 
The following classification models were trained on the balanced training data:
Logistic Regression (with balanced class weight)
XGBoost Classifier
Support Vector Classifier (SVC) with RBF kernel
### Model Evaluation: 
The models were evaluated on the validation set using ROC AUC Score, Confusion Matrix, and Classification Report (Precision, Recall, F1-score).
## Models Used
Logistic Regression
XGBoost Classifier
Support Vector Classifier (SVC)
## Results
The models were evaluated based on their performance on the validation set. The ROC AUC scores were:

Logistic Regression: 0.8166

XGBoost Classifier: 0.6467

SVC: 0.6458
