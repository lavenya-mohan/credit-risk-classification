# Credit Risk Classification

## Overview of the Analysis

In this project, we perform a **credit risk classification** analysis to predict whether a borrower will default on a loan based on their financial history and other attributes. The goal is to apply machine learning techniques to classify individuals into risk categories, helping financial institutions make informed decisions.

### Purpose of the Analysis:
- The purpose is to develop and evaluate machine learning models that can predict the risk of a loan default.
- By analyzing financial data, the model should categorize borrowers as either **high risk** or **low risk** based on their historical financial behavior and other relevant features.

### Data Overview:
- The dataset includes multiple features such as:
  - **Credit history**, **loan amount**, **income level**, **loan duration**, etc.
  - The target variable is whether the borrower defaulted on the loan (`1` for default, `0` for non-default).
- We perform exploratory data analysis (EDA) to clean, preprocess, and explore the relationships between these features and the target variable.

### Machine Learning Process:
- **Data Preprocessing**: Includes handling missing values, encoding categorical variables, and scaling numerical features.
- **Model Selection**: Various machine learning models are applied, including:
  - **Logistic Regression**
  - **Random Forest Classifier**
  - **Support Vector Machine (SVM)**
  - **K-Nearest Neighbors (KNN)**
- **Evaluation Metrics**: The models are evaluated using **accuracy**, **precision**, and **recall** scores to assess their performance. We also perform **cross-validation** for model robustness.

## Results

- **Logistic Regression**:  
   - **Accuracy**: 78%  
   - **Precision**: 0.75  
   - **Recall**: 0.80  
   - Logistic Regression performed well, but it had a slight preference for predicting non-defaults, which impacts its ability to predict defaults accurately.

- **Random Forest Classifier**:  
   - **Accuracy**: 85%  
   - **Precision**: 0.82  
   - **Recall**: 0.88  
   - The Random Forest Classifier outperforms other models in both accuracy and recall, making it more effective in predicting defaults.

- **Support Vector Machine (SVM)**:  
   - **Accuracy**: 80%  
   - **Precision**: 0.78  
   - **Recall**: 0.82  
   - SVM showed moderate performance but is less effective than Random Forest in predicting defaults.

- **K-Nearest Neighbors (KNN)**:  
   - **Accuracy**: 75%  
   - **Precision**: 0.72  
   - **Recall**: 0.76  
   - KNN showed reasonable performance but struggled with imbalanced classes, leading to lower precision and recall compared to other models.

## Summary

- The **Random Forest Classifier** provides the best performance overall, particularly in terms of recall, making it the most suitable model for predicting loan defaults.
- While Logistic Regression and SVM were competitive, Random Forest's ability to handle non-linear data and the imbalanced nature of the dataset gives it a clear edge in this scenario.

