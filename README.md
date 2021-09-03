# Challenge_17_Credit_Risk_Analysis
## Supervised Machine Learning & Credit Risk

### PURPOSE
The purpose of this challenge is to apply machine learning techniques (models) to determine if we can assess credit risk programatically. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans; therefore we will use our models to sample, train and predict credit risk. Lastly we will evaulate the efficacy of each model.

#### The algorithms that we will evaluate are as follows:
1) RandomOverSampler
2) SMOTE
3) ClusterCentroids
4) SMOTEENN
5) BalancedRandomForestClassifier
6) EasyEmsembleClassifier

We will evaluiate the algorithms above using the accuracy score from the sklearn.metrics library. This method compares the actual outcome (y) values from the test set against the model's predicted values. Secondly we will evaluate the models using the classification_report_imbalanced from the imblearn.metrics library to determine the precision and sensitivity (recall) of the given model.


### RESULTS:
#### RandomOverSampler
Fig 1. [https://github.com/klegaultguthrie/Challenge_17_Credit_Risk_Analysis/blob/main/Fig1.png]!

There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models (15 pt)
Summary:

There is a summary of the results (2 pt)
There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)
