Credit Risk Prediction using BNPL Dataset

Task Objective
The objective of this project is to predict whether a customer will default on Buy Now Pay Later (BNPL) payments using machine learning techniques.

This is a binary classification problem, where:

1 → Customer will default
0 → Customer will not default

The goal is to help financial systems identify high-risk customers early and reduce financial losses.


 Approach

To solve this problem, the following steps were performed:
Data Understanding

Loaded BNPL transaction dataset containing 10,345 records
Explored features such as:

Customer demographics (age, employment type, location)
Financial attributes (income, credit score, debt ratio)
Behavioral data (repayment delay, missed payments)
Risk indicators (risk score, customer segment)

Data Preprocessing

Handled missing values:

Numerical features → filled with mean
Categorical features → filled with mode
Removed irrelevant column: user_id
Converted transaction_date into:

year, month, day features

Feature Engineering

Applied Label Encoding for categorical variables
Performed feature scaling using StandardScaler
Split dataset into training (80%) and testing (20%) sets using stratified sampling



Model Building

Two machine learning models were applied:

* Logistic Regression (baseline model)
* Random Forest Classifier (final model)

The Random Forest model was selected for final evaluation due to better performance.

---

Evaluation

Model performance was measured using:

Accuracy Score
Confusion Matrix
Feature Importance Analysis


Results & Insights

Key Findings from Data Analysis

Customers with higher repayment delays are significantly more likely to default
Lower credit scores strongly indicate higher risk
Higher income reduces default probability
Debt-to-income ratio and risk score are strong predictors of financial stability
Behavioral features are more important than demographic features


Model Performance

Final model accuracy: ~71%
Random Forest performed better than baseline Logistic Regression
Confusion matrix showed balanced detection of both default and non-default cases

Most Important Features

Repayment delay days
Missed payments
Credit score
Debt-to-income ratio
Risk score

Final Conclusion

This project demonstrates that customer behavioral patterns are the strongest indicators of financial risk in BNPL systems.

Machine learning models can effectively identify high-risk customers, helping financial institutions reduce default rates and improve decision-making.

Tools & Technologies Used

Python
Pandas & NumPy
Matplotlib & Seaborn
Scikit-learn
Machine Learning (Classification Models)

