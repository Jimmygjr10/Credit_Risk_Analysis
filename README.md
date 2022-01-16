# Credit_Risk_Analysis

## Overview:
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Resources
Software: Python 3.9, Anaconda NAvigator 1.9.12, Conda 4.8.4, Jupyter Notebook 6.0.3

## Results

### Random Over Sample model

![balanced_accuracy](https://user-images.githubusercontent.com/83085800/149665426-31f4d69d-4698-413e-9072-24c2cb2ba2e4.png)
![Credit_risk](https://user-images.githubusercontent.com/83085800/149665427-548064fd-6e84-4c74-937c-a5bc728997cd.png)
![F1-Score](https://user-images.githubusercontent.com/83085800/149665428-c427c8eb-5288-4020-ba43-d0d606b89725.png)

The balanced accuracy score is 64%.
When we look at the classification report the precision at the high risk is low at 1% while low risk precision is at 100%. The F1 score for high risk is 2% while the F1 score for low risk is 81%.
