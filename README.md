# Initial_Capstone
Initial Report of capstone Project "Credit Card fraud Detection"

***Project Overview***

# Predicting Fraudulent Credit Card Transactions

This project focuses on predicting whether a credit card transaction is fraudulent by applying machine learning to historical transaction data. The analysis is designed to identify patterns that separate fraudulent activity from legitimate customer behavior. Detecting fraud accurately is important because it can help reduce financial losses, improve customer confidence, and strengthen fraud prevention systems. The main purpose of this project is to use exploratory data analysis and a baseline model to understand which transaction characteristics are most useful for fraud detection.

***Key Features Considered***

Transaction Amount, Transaction Time, PCA-transformed features (V1 to V28), Fraud Class Label

***Notebooks***

https://github.com/Chaitra013/Initial_Capstone/blob/main/credit_card_fraud_capstone_module20.ipynb


***Data Analysis, Modeling and Insights***
Assignment Objective: Perform exploratory data analysis, clean the dataset, engineer useful features, and build a baseline machine learning model that can be improved in later stages of the capstone.

***Overview***

Exploratory data analysis was carried out on the Credit Card Fraud Detection dataset, followed by the development of a Logistic Regression baseline model to classify fraudulent and legitimate transactions. The analysis included checking for missing values, removing duplicate records, examining class imbalance, studying feature distributions, and reviewing correlations with the fraud label. The baseline model was then evaluated using precision, recall, F1-score, ROC-AUC, and a confusion matrix.

***Key Observations***

The dataset is extremely imbalanced, with fraudulent transactions representing only a very small share of the total records. Duplicate rows were identified and removed during cleaning, which slightly changed the class totals while keeping the imbalance pattern largely unchanged. Exploratory analysis showed that several transformed features had noticeable relationships with the fraud target, even though the original meanings of the PCA-based variables are not directly interpretable. Transaction amount also showed differences between fraudulent and non-fraudulent classes, suggesting that unusual spending behavior may still be informative. The Logistic Regression baseline separated the two classes reasonably well overall, but the confusion matrix reflected the usual tradeoff in fraud detection between identifying more fraudulent transactions and avoiding too many false alerts. Because of the class imbalance, measures such as recall, precision, and F1-score were more meaningful than accuracy by itself.

***Inference***

The baseline Logistic Regression model serves as a useful starting point for fraud detection because it offers an interpretable benchmark for later model comparisons. The exploratory analysis indicates that the dataset contains meaningful signals that can help distinguish fraudulent activity from legitimate transactions, but the heavy class imbalance makes the prediction task challenging. The findings suggest that stronger performance may be possible with additional feature engineering, imbalance-handling methods, and more flexible models such as tree-based classifiers. Even at the baseline stage, the results show that machine learning can support fraud detection by identifying suspicious transaction patterns and helping financial institutions respond more effectively.
