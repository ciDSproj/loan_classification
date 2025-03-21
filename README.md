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


## Dataset
The Loan dataset consists of information on the loan structure, the borrower, and whether the loan was paid back in full. It is provided by the Lending Club, which is a company that connects borrowers with investors.


## Data Cleaning and Preprocessing
- Verify for duplicates and missing values
- Apply logarithm transformation to revolving balance
- Binning categories
- Category encoding (Label encoding)
- Drop redundant columns
- Normalize features (min-max normalization)
- Split the dataset into training and testing sets


## Exploratoru Analysis
- Generated a correlation matrix between the numeric columns and explored how the columns are positively and negatively correlated with each other
- Segmented data by the purpose of the loan and visualized how the relationships between numerical variables change across distinct categories
- Created histograms for numeric columns with a color element to segment the bars by “not_fully_paid” loans
- Analyzed the relationship between loan purpose and different numeric variables for fully paid loans


## Build Classification models
In training and evaluating the models, I accounted for: 
-	 the class imbalance in the target variable  that has fewer examples of loans not fully paid
-	the importance of accurately predicting whether a loan will not be paid back rather than if a loan is paid

I followed the steps below for building the models:
- train a list of models, in this case Logistic Regression, Random Forest and Gradient Boosting
- calculate the evaluation metrics including recall, precision and f1_score
- print out the confusion matrix
- apply SMOTE algorithm (Synthetic Minority Oversampling Technique) by oversampling the minority class on train data, to balance the class distribution
- re-train and re-evaluate the models on resampled data
- compare the results after applying SMOTE
- plot precision-recall curve which allows us to visualize these metrics at various threshold levels and observe the tradeoff between the two



