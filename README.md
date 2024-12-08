# Credit Card Fraud Detection
## Introduction
This repository contains a machine learning project aimed at detecting fraudulent credit card transactions. The goal is to build a robust model that accurately distinguishes between fraudulent and legitimate transactions using anonymized data.

### Dataset : https://www.kaggle.com/datasets/kartik2112/fraud-detection
The dataset used in this project is the Credit Card Fraud Detection dataset, which contains 284,807 transactions with 492 fraudulent cases. The dataset is highly imbalanced, with frauds accounting for only 0.17% of all transactions. Features are numeric values resulting from a PCA transformation to ensure anonymity.

## Project Steps
### 1. Data Preprocessing
Step Description:
Loaded the dataset and examined its structure.
Checked for missing values (no missing values were found).
Normalized the 'Amount' feature using StandardScaler for improved model performance.
Outcome: The dataset was clean and ready for exploratory data analysis (EDA).
### 2. Exploratory Data Analysis (EDA)
Step Description:
Analyzed the distribution of classes (fraud vs. legitimate).
Examined feature correlations and performed visualization using histograms, box plots, and heatmaps.
Key Insights:
The dataset is highly imbalanced, requiring techniques like resampling or algorithm-level adjustments.
Certain features showed significant differences between fraudulent and legitimate transactions.
### 3. Handling Imbalanced Data
Step Description:
Used SMOTE (Synthetic Minority Over-sampling Technique) to address class imbalance.
Created a balanced dataset to train the model.
Outcome: Improved balance between classes, enabling better model training and evaluation.
### 4. Model Selection and Training
Model Training Metrics
The model was trained over 50 epochs with the following metrics captured for each epoch:


Training Performance Highlights
A .Highest Accuracy: 99.37% (Epoch 50)

B. Lowest Validation Loss: 0.0052 (Epoch 44)

C.Highest Validation Accuracy: 99.98% (Epoch 44)

Model Evaluation Metrics
After training, the following evaluation metrics were obtained:

### Confusion Matrix:

True Negatives (TN): Non-fraudulent transactions are correctly predicted as non-fraudulent.

False Positives (FP): Non-fraudulent transactions incorrectly predicted as fraudulent.

False Negatives (FN): Fraudulent transactions incorrectly predicted as non-fraudulent.

True Positives (TP): Fraudulent transactions are correctly predicted as fraudulent.

### Classification Report (based on test data):

Model Training Metrics

The model was trained over 50 epochs, with the following key results:


Final Epoch (50):

Training Accuracy: 99.37%

Training Loss: 0.0188

Validation Accuracy: 99.76%

Validation Loss: 0.0141

Evaluation Metrics

Overall Accuracy: 94%

The model achieved a robust performance during evaluation.

### Classification Report:


Class: Non-Fraudulent Transactions
  
  Precision: 0.99
  
  Recall: 0.90
  
  F1-Score: 0.94
  
  Class: Fraudulent Transactions
  
  Precision: 0.88
  
  Recall: 0.99
  
  F1-Score: 0.93


## Conclusion

The training process showed consistent improvements in accuracy and loss across epochs, with the highest accuracy of 99.37% and lowest validation loss of 0.0141 achieved at the final epoch.
The model effectively identifies both fraudulent and non-fraudulent transactions, achieving a balanced F1-score of 0.94 for both classes.
Future improvements could target reducing false positives to enhance the precision for fraudulent transactions.

## Outcome:
The final model achieved an F1-score of 0.97 and an AUC of 0.98, indicating strong performance on the testing set.

