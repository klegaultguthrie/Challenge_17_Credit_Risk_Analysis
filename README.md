# Challenge_17_Credit_Risk_Analysis
## Supervised Machine Learning & Credit Risk

### PURPOSE
The purpose of this challenge is to apply machine learning techniques (models) to determine if we can assess credit risk programmatically. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans; therefore we will use our models to sample, train and predict credit risk. Lastly we will evaluate the efficacy of each model.

#### The algorithms that we will evaluate are as follows:
1) RandomOverSampler
2) SMOTE
3) ClusterCentroids
4) SMOTEENN
5) BalancedRandomForestClassifier
6) EasyEmsembleClassifier

We will evaluate the algorithms above using the accuracy score from the sklearn.metrics library. This method compares the actual outcome (y) values from the test set against the model's predicted values. Secondly we will evaluate the models using the classification_report_imbalanced from the imblearn.metrics library to determine the precision and sensitivity (recall) of the given model.


### RESULTS:
### RandomOverSampler
Fig 1.

![](https://github.com/klegaultguthrie/Challenge_17_Credit_Risk_Analysis/blob/main/Fig1.png)

Fig 2.

![](https://github.com/klegaultguthrie/Challenge_17_Credit_Risk_Analysis/blob/main/Fig2.png)
* Accuracy = 62%
* Precision:                     
  * Low_risk Loans = 100%
  * High_risk Loans = 1%

* Recall                 
  * Low_risk Loans = 63%
  * High_risk Loans = 61%

### SMOTE Oversampling
Fig 3.

![](https://github.com/klegaultguthrie/Challenge_17_Credit_Risk_Analysis/blob/main/Fig3.png)

Fig 4. 

![](https://github.com/klegaultguthrie/Challenge_17_Credit_Risk_Analysis/blob/main/Fig4.png)
* Accuracy = 62%
* Precision:                     
  * Low_risk Loans = 100%
  * High_risk Loans = 1%

* Recall                 
  * Low_risk Loans = 65%
  * High_risk Loans = 61%

### ClusterCentroids Undersampling
Fig 5. 

![](https://github.com/klegaultguthrie/Challenge_17_Credit_Risk_Analysis/blob/main/Fig5.png)

Fig 6.

![](https://github.com/klegaultguthrie/Challenge_17_Credit_Risk_Analysis/blob/main/Fig6.png)

* Accuracy = 63%
* Precision:                     
  * Low_risk Loans = 99%
  * High_risk Loans = 1%

* Recall                 
  * Low_risk Loans = 42%
  * High_risk Loans = 58%

### Combination (Over and Under) Sampling

Fig 7.

![](https://github.com/klegaultguthrie/Challenge_17_Credit_Risk_Analysis/blob/main/Fig7.png)

Fig 8.

![](https://github.com/klegaultguthrie/Challenge_17_Credit_Risk_Analysis/blob/main/Fig8.png)

* Accuracy = 50%
* Precision:                     
  * Low_risk Loans = 100%
  * High_risk Loans = 1%

* Recall                 
  * Low_risk Loans = 58%
  * High_risk Loans = 71%

#### Balanced Random Forest Classifier

Fig. 9

![](https://github.com/klegaultguthrie/Challenge_17_Credit_Risk_Analysis/blob/main/Fig9.png)

Fig 10.
![](https://github.com/klegaultguthrie/Challenge_17_Credit_Risk_Analysis/blob/main/Fig10.png)

* Accuracy = 77%
* Precision:                     
  * Low_risk Loans = 100%
  * High_risk Loans = 3%

* Recall                 
  * Low_risk Loans = 88%
  * High_risk Loans = 66%


#### Easy Ensemble AdaBoost Classifier

Fig 11.

![](https://github.com/klegaultguthrie/Challenge_17_Credit_Risk_Analysis/blob/main/Fig11.png)

Fig 12.

![](https://github.com/klegaultguthrie/Challenge_17_Credit_Risk_Analysis/blob/main/Fig12.png)

* Accuracy = 93%
* Precision:                     
  * Low_risk Loans = 100%
  * High_risk Loans = 9%

* Recall                 
  * Low_risk Loans = 95%
  * High_risk Loans = 92%

### SUMMARY & RECOMENDATION:

There was little variance in the accuracy results of the Random and Smote oversampling and the ClusterCentroids undersampling models. The Combination sampling model performed the worst with an accuracy score of only 50%. The Easy EnsembleAdaboost Classifier model performed by in large the best with an accuracy score of 93%, followed by the Balanced Random Forest Classifier at 77%. With regards to the precision and recall scores of the models, the Easy EnsembleAdaboost also performed the best; consequently, this is the model that is recommended.
