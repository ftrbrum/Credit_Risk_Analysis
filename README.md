# Credit_Risk_Analysis
Module 17


## Overview of Analysis:

We are going to apply machine learning to solve the real world challenge of credit card risk.  Credit risk is an unbalanced classification problem as good loans easily outnumber risky loans.  We will employ different techniques to train and evaluate models with unbalanced classes using imbalanced-learn and scikit-learn libraries to build and evaluate the models with resampling.  We will oversample our data using RandomOverSampler and SMOTE algorithms and undersample the data with the ClusterCentroids algorithm.  Next we will use a combinatorial approach of over and undersampling using the SMOTEENN algorithm.  That will be followed by compare two machine learning models, BalancedRandomForestClassifier and EasyEnsembleClassifier, that reduce bias to predict credit risk.


## Resources:

Software:<br/> 
VS Code version 1.59
Python version 3.7.10
 
Code:<br/> 
[credit_risk_resampling.ipynb](Challenge/credit_risk_resampling.ipynb)<br/>
[credit_risk_ensemble.ipynb](Challenge/credit_risk_ensemble.ipynb)<br/>

Images:<br/>
[Images](Challenge/Images/) <br/>

Data:<br/>
[LoanStats_2019Q1.csv](Challenge/Resources/LoanStats_2019Q1.csv)<br/>


## Results:

Naive Random Oversampling
![oversampling_imbalanced.png](Challenge/Images/oversampling_imbalanced.png) <br/>

SMOTE Oversampling
![SMOTE_oversampling_imbalanced.png](Challenge/Images/SMOTE_oversampling_imbalanced.png) <br/>

Cluster Centroids
![undersampling_imbalanced.png](Challenge/Images/undersampling_imbalanced.png) <br/>

SMOTEENN
![over_under_sampling_imbalanced.png](Challenge/Images/over_under_sampling_imbalanced.png) <br/>

Balanced Random Forest Classifier
![random_forest_imbalanced.png](Challenge/Images/random_forest_imbalanced.png) <br/>

Easy Ensemble AdaBoost Classifier
![easy_ensemble_imbalanced.png](Challenge/Images/easy_ensemble_imbalanced.png) <br/>


## Summary:

