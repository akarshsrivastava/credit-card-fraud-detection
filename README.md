# credit-card-fraud-detection

Credit card fraud and scams have increased significantly in the last decade. The technological advancement has provided such fraudsters new means and tactics to commit such crimes. Such frauds and scams cost consumers and the financial company large sums of dollars annually. Thus, fraud detection systems have become essential for banks and financial institution, to minimize their losses.

Technological advancements in the field of machine learning and deep learning have proven themselves very helpful in detecting and predicting such anomalies. So, for this project, I will attempt to build a supervised learning model which could detect such anomalies in transactions and help in reducing such crimes.

Python Notebook: https://github.com/akarshsrivastava/credit-card-fraud-detection/blob/main/credit-card-fraud-detection.ipynb

Dataset:

1. For this project, I have taken the credit card dataset from Kaggle.com

URL: https://www.kaggle.com/mlg-ulb/creditcardfraud

2. The datasets contains transactions made by credit cards in September 2013 by european cardholders.

3. The data set is highly skewed, consisting of 492 frauds in a total of 284,807 observations. This resulted in only 0.172% fraud cases. This reflect the real life scenarios where the fraud transactions will be very less compared to regular transactions. So we need a model which take this imbalance into account.

4. The dataset consists of numerical values from the 28 ‘Principal Component Analysis (PCA)’ transformed features, namely V1 to V28. Furthermore, there is no metadata about the original features provided, so pre-analysis or feature study could not be done.

5. The ‘Time’ and ‘Amount’ features are not transformed data. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

6. There is no missing value in the dataset.

Approach:

As we know our data is imbalanced, we need to keep this in mind while training our model. I will build 4 model using different approaches:
1. Logistic Regression based model using Grid search for hyper parameter tuning
2. Random Forest Classifier based model with grid search for hyper parameter tuning
3. Using under sampling to lessen the gap between entries of class 1 and 0 by reducing the class 0 entries. Further, we use Random Forest for training
4. Using over sampling to lessen the gap between entries of class 1 and 0 by increasing the class 1 entries. Further, we use Random Forest for training


 
