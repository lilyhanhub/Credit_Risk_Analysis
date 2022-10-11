# Credit_Risk_Analysis
## Overview of the project
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. The purpose of this project is to perform six different machine learning models to analyze credit card risk, evaluate the performance of these models, and make recommendations on whether they should be used to predict credit risk. The project consists of three tasks:
* Use resampling models to predict credit risk
    * Oversample the data: RandomOverSampler and SMOTE algorithms
    * Undersample the data: ClusterCentroids algorithm
* Use the combinatorial approach of over- and undersampling SMOTEENN algorithm to predict credit risk
* Use ensemble classifiers to predict credit risk
    * BalancedRandomForestClassifier algorithm
    * EasyEnsembleClassifier algorithm

## Results
There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models (15 pt)
### I. RandomOverSampler
![RandomOverSampleing](Resources/images/RandomOverSampling.png)


### II. SMOTE Oversampling
![SMOTE](Resources/images/SMOTE.png)


### III. ClusterCentroids Undersampling
![UnderSampling](Resources/images/UnderSampling.png)


### IV. SMOTEENN Combination Sampling
![SMOTEENN](Resources/images/SMOTEENN.png)

### V. Balanced Random Forest Classifier
![BRFensemble](Resources/images/BRFensemble.png)

### VI. Easy Ensemble Classifier
![EasyEnsembleClassifier](Resources/images/EasyEnsembleClassifer.png)


## Summary
There is a summary of the results (2 pt)
There is a recommendation on which model to use, or there is no recommendation with a justification