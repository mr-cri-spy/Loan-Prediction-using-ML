# Loan-Prediction-using-ML

Loan Approval Predictor  Predicting the Future of Borrowers with ML

Project Objectives:
  *Predict whether a loan should be approved or not based on customer financial data.
  *Use logistic regression for classification.
  *Gain insights into financial behavior of applicants.
  *Create an end-to-end ML pipeline with data preprocessing, training, evaluation, and deployment-ready prediction.

Tools & Libraries:
Python , scikit-learn , pandas  , matplotlib / seaborn (for visualization)

**Loan Prediction Using Machine Learning**
Welcome:) This project uses customer financial information to predict whether a loan should be approved or not. It's built using a logistic regression model and demonstrates a real-world classification problem with practical use in banks and financial services.


**Project Overview**
This project aims to predict whether a loan application will be approved or rejected based on applicant details like income, employment status, credit history, and other financial indicators. It simulates a real world classification problem that banks and financial institutions face daily, where quick and accurate loan approval decisions are essential.

The model is built using Logistic Regression, a simple yet powerful algorithm suitable for binary classification tasks. The goal is to identify patterns from historical data and use those patterns to make reliable future predictions.  

 Key Features;-
      
        End-to-end ML pipeline: from data cleaning to prediction.
        Real-world dataset used for modeling.
        Custom sample prediction for new applicants.
        Preprocessing using one-hot encoding and handling of missing data.
        Model evaluation using accuracy, confusion matrix, and classification report.


Dataset Information:- 

 We used a publicly available dataset related to loan applications. It includes features like:
   Gender, Marital Status, Dependents
   Education, Selfemployment status
   Applicant & Co applicant Income
   Loan amount & Loan term
   Credit history
   Property area
   Loan Status (Target Variable)

Data Preprocessing
    Handled missing values using mode/median strategies.
    Dropped irrelevant columns like Loan_ID.
    Encoded categorical variables using one hot encoding.
    Final feature set includes both numerical and binary categorical features post encoding.

Model Building
   Used Logistic Regression for binary classification.
   Split data into training and testing sets (80/20 ratio).
   Trained the model and evaluated using:
  * Accuracy Score
  * Confusion Matrix
   * Classification Report


Model Evaluation Output Should Be :-

Accuracy Score: 0.XX

 Confusion Matrix:
   [[18  4]
   [ 4  9]]

Classification Report:
              precision    recall  f1-score   support

           0       0.82      0.82      0.82        22
           1       0.69      0.69      0.69        13

    accuracy                           0.78        35
   macro avg       0.76      0.76      0.76        35
weighted avg       0.78      0.78      0.78        35


Sample Prediction for New Customer
We crafted a manual input array to simulate a new loan applicant’s profile:-- 

sample = np.array([[5000, 0.0, 150.0, 360.0, 1.0,  # Numeric features
                    1, 1,  # Gender_Male, Married_Yes
                    0, 0, 0,  # Dependents_1, Dependents_2, Dependents_3+
                    0,  # Education_Not Graduate
                    0,  # Self_Employed_Yes
                    0, 1]]) # Property_Area_Semiurban, Property_Area_Urban

                         Prediction (1=Approved, 0=Rejected):", model.predict(sample)[0]

   Prediction Result : 1 → Loan Approved

This project demonstrates how machine learning can be used to automate and improve decision making in the finance domain. While we’ve started with logistic regression, this system can be expanded to include more advanced models, automated feature selection, and model explainability techniques like SHAP or LIME for real world deployment.

We can XGBoost or Random Forest for better performance lets do it later





