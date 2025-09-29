# Logistic Regression on Breast Cancer Dataset

## Overview
This project implements a **binary classification model** using **Logistic Regression** on the Breast Cancer Wisconsin dataset.  
The goal is to predict whether a tumor is **Malignant (cancerous)** or **Benign (non-cancerous)** based on medical diagnostic features.

## Steps Performed
1. **Data Preparation**
   - Loaded the dataset (`data.csv`).
   - Dropped unnecessary columns: `id`, `Unnamed: 32`.
   - Defined **features (X)** as all numeric columns.
   - Defined **target (y)** as the `diagnosis` column (mapped: `M = 1`, `B = 0`).

2. **Train-Test Split**
   - Split the dataset into training (80%) and testing (20%) sets using `train_test_split`.
   - Used `stratify=y` to maintain class balance.

3. **Feature Scaling**
   - Standardized the features using `StandardScaler` for better model performance.

4. **Model Training**
   - Trained a **Logistic Regression** model on the training set.

5. **Evaluation**
   - Made predictions on the test set.
   - Evaluated using:
     - Confusion Matrix
     - Accuracy, Precision, Recall, F1-score
   - Plotted **ROC curve** and calculated **AUC**.

## Results
- The Logistic Regression model successfully classified tumors as malignant or benign.
- Evaluation metrics and ROC-AUC confirmed strong performance.
