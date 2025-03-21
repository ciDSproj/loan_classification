# Loan Classification
The goal of this project was to build a classifier to predict whether a loan will be paid back, based on a dataset containing information on the loan structure and the borrower. After a thorough data analysis, I built several classification models. In training and evaluating the model, I accounted for the class imbalance in the target variable  that has fewer examples of loans not fully paid.


## Overview
It is a well-known fact that in the loan lending industry it's more important to accurately predict whether a loan will not be paid back rather than if a loan is paid back. Failing to detect loan defaulters can lead to significant financial risk for the institution. A thorough analysis of what causes loan faults and how to predict them can be used to build and maintain financial health and foster trust with both customers and stakeholders.


## Resources Used
- Python 3.7
- NumPy and Pandas for data manipulation
- Matplotlib and Seaborn for data visualization
- collections (Counter) to summarize the target class distribution
- imbalanced-learn (SMOTE) to address class imbalance
- sklearn for preprocessing and scaling, train_test_split data and building the classification models


