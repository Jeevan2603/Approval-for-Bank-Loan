Bank Personal Loan Modeling
This repository contains the code and analysis for predicting personal loan approvals based on customer data. The project involves exploratory data analysis (EDA), data visualization, statistical testing, and building several machine learning models to identify the best predictive model.

Table of Contents
Project Overview
Dataset
Exploratory Data Analysis
Data Preprocessing
Statistical Analysis
Model Building
Results
Conclusion
Dependencies
Usage
Project Overview
The objective of this project is to predict whether a customer will accept a personal loan offer. The project uses a dataset provided by a bank, containing various customer attributes. The analysis includes:

Data cleaning and preprocessing
Exploratory data analysis (EDA)
Visualizations to understand data distributions and relationships
Statistical tests to determine feature importance
Building and evaluating multiple machine learning models
Dataset
The dataset Bank_Personal_Loan_Modelling.csv contains 5000 records and 14 attributes:

ID: Customer ID
Age: Customer's age in years
Experience: Years of professional experience
Income: Annual income in $000
ZIP Code: Home address ZIP code
Family: Family size
CCAvg: Average spending on credit cards per month ($000)
Education: Education level (1: Undergrad, 2: Graduate, 3: Advanced/Professional)
Mortgage: Value of house mortgage if any ($000)
Personal Loan: Did the customer accept the personal loan offer? (1: Yes, 0: No)
Securities Account: Does the customer have a securities account? (1: Yes, 0: No)
CD Account: Does the customer have a certificate of deposit (CD) account? (1: Yes, 0: No)
Online: Does the customer use internet banking? (1: Yes, 0: No)
CreditCard: Does the customer use a credit card issued by the bank? (1: Yes, 0: No)
Exploratory Data Analysis
The initial EDA included:

Viewing the first few records
Checking for missing values
Analyzing unique values for categorical variables
Generating descriptive statistics
Visualizing distributions and relationships using pair plots and heatmaps
Data Preprocessing
The preprocessing steps included:

Dropping irrelevant columns (ID and ZIP Code)
Handling negative values in the Experience column by converting them to their absolute values
Creating categorical bins for continuous variables (e.g., income)
Statistical Analysis
Chi-square tests were conducted to determine the dependency of personal loan acceptance on various features such as income and education. The results indicated significant dependencies, which were visualized using box plots.

Model Building
Several models were trained and evaluated:

Logistic Regression
Naive Bayes
K-Nearest Neighbors (KNN)
Logistic Regression
Achieved the highest accuracy (95.13%)
Low Type I and Type II errors
Naive Bayes
Accuracy: 88.00%
Higher error rates compared to Logistic Regression
K-Nearest Neighbors (KNN)
Optimal K value determined through error rate analysis
Accuracy: 91.07% at K=8
Results
The Logistic Regression model outperformed other models with an accuracy of 95.13%, making it the best choice for predicting personal loan acceptance.

Conclusion
Logistic Regression is the most effective model for this dataset due to its high accuracy and low error rates. The project demonstrates the importance of thorough EDA, statistical analysis, and model evaluation in predictive modeling.

Dependencies
pandas
numpy
seaborn
matplotlib
scikit-learn
scipy
