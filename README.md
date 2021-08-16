# Credit_Risk_Analysis
Module 17


## Overview of Analysis:

We are going to apply machine learning to solve the real world challenge of credit card risk.  Credit risk is an unbalanced classification problem as good loans easily outnumber risky loans.  We will employ different techniques to train and evaluate models with unbalanced classes using imbalanced-learn and scikit-learn libraries to build and evaluate the models with resampling.  We will oversample our data using RandomOverSampler and SMOTE algorithms and undersample the data with the ClusterCentroids algorithm.  Next we will use a combinatorial approach of over and undersampling using the SMOTEENN algorithm.  That will be followed by compare two machine learning models, BalancedRandomForestClassifier and EasyEnsembleClassifier, that reduce bias to predict credit risk.


## Resources:

Software:<br/> 
VS Code version 1.59<br/>
Python version 3.7.10<br/>
 
Code:<br/> 
[credit_risk_resampling.ipynb](Challenge/credit_risk_resampling.ipynb) <br/>
[credit_risk_ensemble.ipynb](Challenge/credit_risk_ensemble.ipynb) <br/>

Images:<br/>
[Images](Challenge/Images/) <br/>

Data:<br/>
[LoanStats_2019Q1.csv](Challenge/Resources/LoanStats_2019Q1.csv) <br/>


## Results:

Naive Random Oversampling <br/>
![oversampling_imbalanced.png](Challenge/Images/oversampling_imbalanced.png) <br/>
- Balanced Accuracy Test is 64.9%<br/>
- Precision Score average total is 99%<br/>
- Recall Score average total is 40%<br/>

SMOTE Oversampling <br/>
![SMOTE_oversample_imbalanced.png](Challenge/Images/SMOTE_oversample_imbalanced.png) <br/>
- Balanced Accuracy Test is 65.8%<br/>
- Precision Score average total is 99%<br/>
- Recall Score average total is 68%<br/>

Cluster Centroids <br/>
![undersampling_imbalanced.png](Challenge/Images/undersampling_imbalanced.png) <br/>
- Balanced Accuracy Test is 65.8%<br/>
- Precision Score average total is 99%<br/>
- Recall Score average total is 40%<br/>

SMOTEENN <br/>
![over_under_sampling_imbalanced.png](Challenge/Images/over_under_sampling_imbalanced.png) <br/>
- Balanced Accuracy Test is 54.4%<br/>
- Precision Score average total is 99%<br/>
- Recall Score average total is 58%<br/>

Balanced Random Forest Classifier <br/>
![random_forest_imbalanced.png](Challenge/Images/random_forest_imbalanced.png) <br/>
- Balanced Accuracy Test is 74.7%<br/>
- Precision Score average total is 99%<br/>
- Recall Score average total is 88%<br/>

Easy Ensemble AdaBoost Classifier <br/>
![easy_ensemble_imbalanced.png](Challenge/Images/easy_ensemble_imbalanced.png) <br/>
- Balanced Accuracy Test is 93.1%<br/>
- Precision Score average total is 99%<br/>
- Recall Score average total is 94%<br/>


## Summary:

We used oversampling in the first 2 models (Naive Random Oversampling and SMOTE Oversampling).  In the third model (Cluster Centroids) we used undersampling.  For the fourth model (SMOTEENN) we used a combination of over and undersampling.  This was to determine which model is best to predict which loans are the highest risk.

In the fifth and sixth models (Balanced Random Forest Classifier and East Ensemble AdaBoost Classifier) we used classifiers to predict which loans are high risk and low risk.

With the first four models, the accuracy score is not as high as the classifiers and the recall in the oversampling, undersampling, and over/undersampling models is low. In the models we wanted a good balance of recall and precision which is why we recommend using the classifiers over the first four models.