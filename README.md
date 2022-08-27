# Credit_Risk_Analysis

## Analysis Overview
In this project an evaluation of several machine learning models was conducted in order to predict credit risk.

The Following models were developed and compared:

1. Oversampling models were conducted using the RandomOverSampler and SMOTE algorithms.
2. UnderSampling model was conducted using the ClusterCentroids algorithm.
3. The SMOTEENN algorithm was used in order to attain a combined oversampling  and undersampling model 
4. Lastly, BalancedRandomForestClassifier and EasyEnsembleClassifier algorithms were used in order to compare two machine learning models.

The performance of these models was analyzed and compared and a recommendation developed for the more appropriate model to predict credit risk.

## Results:

All models were compared on the basis of the same measured matrix which included;  Balanced Accuracy Scores, Confusion Matrixes and Imbalanced Classification Reports

### RandomOverSampler model

!https://github.com/AnaMMoreira/Credit_Risk_Analysis/blob/main/random_oversampling.png

The RandomOverSampler model balanced accuracy score is 64%.
The high-risk precision is about 1% only with 62% sensitivity with a F1 of 2% only.
The low-risk population which had more data points was better represented and its precision is almost 100% with a sensitivity of 65%.


### SMOTE model

!https://github.com/AnaMMoreira/Credit_Risk_Analysis/blob/main/SMOTE_Oversampling.png

The SMOTE model results are pretty similar to the previous model.
The balanced accuracy score is 63%.
The high-risk precision is about 1% with 62% sensitivity with a F1 of 2% only.
The low-risk population which had more data points was better represented and its precision  is almost 100% with a sensitivity of 64%.

### ClusterCentroids model

!https://github.com/AnaMMoreira/Credit_Risk_Analysis/blob/main/Undersampling.png

Undersampling model using the ClusterCentroid algorithm,
the balanced accuracy score is down to about 52%.
The high-risk precision is still 1% with a slightly lower sensitivity of 60% with a F1 of 1%.
The low-risk sensitivity is only 44%.

### Combination model

!https://github.com/AnaMMoreira/Credit_Risk_Analysis/blob/main/Combination_Over_n_Undersampling.png

For theCombination Over-UnderSampling model using SMOTEENN
The balanced accuracy score is about 62%.
The high-risk precision is still 1%, with 71% sensitivity and a F1 of only 2%.
And the low-risk sensitivity is at 54%.

### BalancedRandomForestClassifier model

!https://github.com/AnaMMoreira/Credit_Risk_Analysis/blob/main/Balanced_Random_Forest_Classifier.png

For the Machine learning BalancedRandomForestClassifier model
The balanced accuracy score improved to 79%.
The high-risk precision is still low at 4% only with 67% sensitivity and a F1 of only 7%.
The low-risk sensitivity is increased to 91% with a 99% precision.

### EasyEnsembleClassifier model

!https://github.com/AnaMMoreira/Credit_Risk_Analysis/blob/main/AdaBoost_Classifier.png

The EasyEnsembleClassifier model using the AdaBoost machine learning algorithm
performed the best with a balanced accuracy score of about 93%.
The high-risk precision is still low at 7% only with 91% sensitivity with a F1 of 14%.
The low-risk sensitivity is now 94% with 100% precision.

## Summary
All the models used to perform the credit risk analysis show weak precision in determining high risk credit but perform at a more conservative sensitivity.
The Machine Learning models yielded better results for sensitivity of high-risk credit therefore potentially being better models to flag "bad" investments.
The EasyEnsembleClassifier model in particular showed a balanced accuracy score of 92% so it detects almost all high-risk credit. However, the low precision will falsely detect low risk credits as high risk which could negatively impact the bank's credit revenue performance by being overconservative with business opportunities.
For those reasons a recommendation to use the EasyEnsembleClassifier model in order to identify high-risk credit but perhaps utilize a more reliable model for the low-risk segment of the population.
