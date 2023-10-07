# Credit_Card_Fraud_Detection - Classification Project 


## Introduction

Welcome to the Credit Card Fraud Detection Project, a data-driven initiative aimed at safeguarding financial transactions and protecting users from fraudulent activities. In a world where digital payments have become an integral part of our daily lives, the need for robust security measures has never been greater. This project addresses this challenge by employing cutting-edge machine learning techniques to identify and prevent credit card fraud.

## Dataset Information

The dataset contains transactions made by credit cards in September 2013 by European cardholders.

This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

Given the class imbalance ratio, we recommend measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC). Confusion matrix accuracy is not meaningful for unbalanced classification.

#Link Kaggle of dataset: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud


## Problems
Credit Card Fraud Detection is a classic class-imbalance problem where the number of fraud transactions is much lesser than the number of legitimate transaction for any bank. Most of the approaches involve building model on such imbalanced data, and thus fails to produce results on real-time new data because of overfitting on training data and a bias towards the majoritarian class of legitimate transactions. Thus, we can see this as an anomaly detection problem.

## Goals of the Project

We want to answer questions like:
1. At what time does the Credit Card Frauds usually take place?
2. What are the general trends of amounts for Credit Card Fraud Transactions?
3. How do we balance the data to not let the model overfit on legitimate transactions?

## Libraries

* Pandas ( `pip install pandas` )
* Numpy ( `pip install pandas` )
* Matplotlib ( `pip install matplotlib` )
* Seaborn ( `pip install seaborn` )
* Sklearn ( `pip install sklearn` )
* Imblearn ( `pip install imblearn` )

## Algorithms

* Logistic Regression
* KNeighborsClassifier
* SGDClassifier

## License

This project is licensed under the MIT License. See the LICENSE file for details.
