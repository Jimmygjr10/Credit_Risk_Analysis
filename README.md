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

### SMOTE model

![SMOTE-model](https://user-images.githubusercontent.com/83085800/149665724-7bfd42d6-4035-4ddb-9a96-e5010f2ff5d1.png)

The balanced accuracy score is 62%.
Similar to the random over samole model the low risk precision is 100%, while high risk is only 2%.

### ClusterCentroidsModel

![ClusterCentroid](https://user-images.githubusercontent.com/83085800/149666040-9ba314f8-1d93-4e47-a65b-1b3cd80a8c43.png)

The blalanced accuracy score is at 52%.
The F1 score for low risk is at 60% and for high risk it is at 1%.

### SMOTEEN model

![SMOTEEN](https://user-images.githubusercontent.com/83085800/149666153-e2804563-3a95-4327-9ddb-5360752d9e17.png)

Again the classification report is showing low risk F1 score of 70% with the high risk at 2%.

### BalancedRandomForestClassifier model

![BalancedRandomForestClassifier](https://user-images.githubusercontent.com/83085800/149666459-25aa5f64-0a37-4107-b47c-ce3a8f2a8f26.png)

As we take a look at the classification report for the BalancedRandomForest we see an increase in the F1 score for both low risk and high. Still high risk score is still low their is improvement with this model.

### EasyEnsembleClassifier

![EnsembleClassifier](https://user-images.githubusercontent.com/83085800/149666965-2d8167f4-26b8-45df-86d8-2b005e2cce16.png)

As you an see in this classification report we were able to get even more of an icrease for the F1 score for low risk and high risk!

## Summary

None of the models were able to show strong F1 scores for high risk resulting in precision and sensitivity combined being weak. The best omodel of all with what we had to work with was the EnsembleClassifier. With that being said I would recommend we find a differnet model that will help result in both high F1 scores for both high and low risk. Also try finding another dataset to work on as well.
