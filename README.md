# 🏦 Loan Approval Prediction

This project builds a machine learning pipeline to predict whether a loan application will be approved based on applicant details such as income, credit history, employment, and more. It includes data cleaning, visualization, feature engineering, multiple classification models, and techniques to handle class imbalance.

# 📌Problem Statement
Loan default or delay impacts financial institutions. This project helps predict loan approval status to improve decision-making by automating risk assessment using historical data.

# Dataset Overview
The dataset includes features like:

ApplicantIncome

CoapplicantIncome

LoanAmount

Loan_Amount_Term

Credit_History

Gender, Married, Education, Self_Employed, Property_Area

Loan_Status (Target)

# 🔧 Data Preprocessing Steps
Handled missing values (mean/median/mode based imputation).

Feature transformation using logarithmic scaling.

Combined applicant and co-applicant income into a single feature.

Removed redundant features (Loan_ID, original income columns).

Label encoding of categorical features.

# 📈 Exploratory Data Analysis
Used seaborn and matplotlib to visualize:

Gender/Married/Education distribution.

Boxplots for outliers.

Correlation heatmaps of numerical features.

# 🤖 Machine Learning Models
Evaluated and compared the performance of:

Model	Description
Logistic Regression	Simple linear classifier
Decision Tree	Tree-based split model
Random Forest	Ensemble of decision trees
K-Nearest Neighbors	Distance-based classifier

Metrics used: Accuracy, Confusion Matrix, Cross-validation score.

# ⚖️ Handling Imbalanced Data
Used RandomOverSampler from imblearn to balance class distribution.

# Retrained all models on the balanced dataset for improved recall and F1-score.
| 🧠 Model               | 🎯 Accuracy |
| ---------------------- | ----------- |
| 🧮 Logistic Regression | \~82%       |
| 🌳 Decision Tree       | \~76%       |
| 🌲 Random Forest       | \~84%       |
| 👣 KNN (k=6)           | \~78%       |


