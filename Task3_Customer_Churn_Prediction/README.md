Customer Churn Prediction (Bank Customers)
Project Objective

The objective of this project is to predict whether a bank customer will leave the bank (churn) or continue using its services.

Customer churn prediction is a supervised machine learning classification problem, where the target variable indicates customer retention status:

1 → Customer has churned
0 → Customer has stayed

This project helps banks identify at-risk customers and take proactive retention actions.

Dataset Overview

The dataset contains 10,000 customer records with demographic, financial, and behavioral attributes.

Key Features:
CreditScore → Customer credit rating
Geography → Country (France, Spain, Germany)
Gender → Male / Female
Age → Customer age
Tenure → Number of years with the bank
Balance → Account balance
NumOfProducts → Number of bank products used
HasCrCard → Credit card ownership
IsActiveMember → Activity status
EstimatedSalary → Income estimate
Exited → Target variable (churn or not)
Approach

The project follows a complete machine learning pipeline:

1.  Data Understanding
Loaded dataset from CSV file
Explored shape, structure, and data types
Checked for missing values (none found)
2.  Data Cleaning
Removed irrelevant columns:
RowNumber
CustomerId
Surname

These columns do not contribute to prediction and may introduce noise.

3. Exploratory Data Analysis (EDA)

EDA was performed to understand customer behavior patterns.

 Churn Distribution
Dataset is imbalanced (more non-churn customers)
Gender vs Churn
Female customers show slightly higher churn tendency
 Geography vs Churn
Customers from Germany have higher churn rates
 Age Distribution
Majority of customers are middle-aged
4.  Data Preprocessing

To prepare data for machine learning:

Label Encoding applied to Gender
One-Hot Encoding applied to Geography
Dataset split into training and testing sets (80/20 split)
Feature scaling applied using StandardScaler for numerical stability
5.  Model Building

A Random Forest Classifier was used for prediction.

Why Random Forest?
Handles non-linear relationships well
Works efficiently on tabular datasets
Provides feature importance insights
Reduces overfitting using ensemble learning
Model Evaluation

The model was evaluated using:

Accuracy Score
Confusion Matrix
ROC-AUC Score
Feature Importance Analysis
 Results:
Accuracy: ~86.6%
ROC-AUC Score: ~0.71
 Key Insights

From analysis and model results, the following insights were observed:

Age is one of the strongest predictors of churn
Customers from Germany have significantly higher churn rates
Inactive members are more likely to leave the bank
Lower credit scores increase churn probability
Higher account balance does not always guarantee retention
Feature Importance

The most influential features in predicting churn were:

Age
IsActiveMember
Credit Score
Balance
Geography

These features strongly impact customer retention behavior.

Conclusion

This project successfully developed a machine learning-based churn prediction system.

Steps completed:
Data cleaning and preprocessing
Exploratory data analysis (EDA)
Feature encoding and scaling
Model training using Random Forest
Performance evaluation and interpretation
Final Outcome:

The model can help banks:

Identify customers at risk of leaving
Improve customer retention strategies
Make data-driven business decisions
Tools & Technologies Used
Python
Pandas & NumPy
Matplotlib & Seaborn
Scikit-learn
Machine Learning (Random Forest Classifier)
Final Note

This project demonstrates a complete end-to-end machine learning workflow for a real-world banking problem.
