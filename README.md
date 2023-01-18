# Credit_Risk_Analysis


## Overview Of the Project

The purpose of this project is to evaluate the performance of six different supervised machine learning models to predict credit risk on credit card dataset from LendingClub, a peer to peer lending services company. Credit risk dataset is an unbalanced dataset since good credits outnumber risky credits. Therefore, in the first deliverable of this project, we used diffetent resampling methods to train and evaluate models with unbalanced classes.
In the second deliverable of this project, Balanced Random Forest Classifier and Easy Ensemble Classifier machine learning models were applied to the dataset to predict credit risk. By evaluating each of this models, we identify the best model for predicting the credit risk.
The six models used for this project are as follow:
- Oversampling with `RandomOverSampler`
- Oversampling with `SMOTE`
- Undersampling with `ClusterSentroids`
- Combination of over and under sampling using `SMOTEENN` module
-  `BalancedRandomClassifier`
-  `EasyEnsembleClassifier`

## Results 

1- # Naive Random Oversampling

![](/Images/Naive_oversampling.PNG)

 - Balanced Accuracy Score: 65.73%
 - "High Risk" Rates: Precision Rate = 1% and the Sensitivity/ Recall = 71%.
 - "Low Risk" Rates: Precision Rate = 100% and the Sensitivity/ Recall = 60%.


2- # SMOTE

![](/Images/SMOTE.PNG)

 - Balanced Accuracy Score: 66.22%
 - "High Risk" Rates: Precision Rate = 1% and the Sensitivity/ Recall = 63%.
 - "Low Risk" Rates: Precision Rate = 100% and the Sensitivity/ Recall = 69%.


3- # Undersampling with Clustercentroid

![](/Images/Clustercentroids.PNG)

 - Balanced Accuracy Score: 54.42%
 - "High Risk" Rates: Precision Rate = 1% and the Sensitivity/ Recall = 69%.
 - "Low Risk" Rates: Precision Rate = 100% and the Sensitivity/ Recall = 40%.
 
 
4- # SMOTEENN

![](/Images/SMOTEENN.PNG)

 - Balanced Accuracy Score: 63.92%
 - "High Risk" Rates: Precision Rate = 1% and the Sensitivity/ Recall = 70%.
 - "Low Risk" Rates: Precision Rate = 100% and the Sensitivity/ Recall = 58%.

5- BalancedRandomClassifier

![](/Images/Balancedrandomforestclassifier.PNG)

 - Balanced Accuracy Score: 78.85%
 - "High Risk" Rates: Precision Rate = 3% and the Sensitivity/ Recall = 70%.
 - "Low Risk" Rates: Precision Rate = 100% and the Sensitivity/ Recall = 87%.
 
6- EasyEnsembleClassifier

[](/Images/Easyensembleclassifier.PNG)

 - Balanced Accuracy Score: 93.16%
 - "High Risk" Rates: Precision Rate = 9% and the Sensitivity/ Recall = 92%.
 - "Low Risk" Rates: Precision Rate = 100% and the Sensitivity/ Recall = 94%.
 
 
## Summary

By looking at the results of the above models, it's noticeable that all six models have a 100% precision rate for "Low risk" credits. However, the first four models have a precision rate of 1% for "High Risk" credits and this precision will go higher to 3% and 9% by using the `BalancedRandomClassifier` and `EasyEnsembleClassifier` respectively.
Moreover, the `EasyEnsembleClassifier` has the highest balanced accuracy score of 93.17% compared to the `BalancedRandomClassifier` with a balanced accuracy score of 78.85% and the other four models ranging from 54.42% to 66.22%. Additionally, this model has the highest sensitivity rate of 90% compared to all other models. 
Considering all the factors we can conclude that `EasyEnsembleClassifier`has the best results in predicting credit risk compared to other models and is the most reliable to use for predicting credit risk. 


