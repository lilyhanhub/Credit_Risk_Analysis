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
### I. RandomOverSampler
![RandomOverSampleing](Resources/images/RandomOverSampling.png)
* The balanced accuracy score is 65%.
* For high risk credits, the precision score is 1%, and the recall is 63%, which means only 1% of the predicted high risk credits are true high risk and 63% of the high risk credits are identified by this model. The F1 score is also quite low (0.02). 

### II. SMOTE Oversampling
![SMOTE](Resources/images/SMOTE.png)
* The balanced accuracy score is 61.8%.
* For high risk credits, the precision score is 1%, and the recall is 59%, which means only 1% of the predicted high risk credits are true high risk and 59% of the high risk credits are identified by this model. The F1 score is also quite low (0.02). 

### III. ClusterCentroids Undersampling
![UnderSampling](Resources/images/UnderSampling.png)
* The balanced accuracy score is 51%.
* For high risk credits, the precision score is 1%, and the recall is 59%, which means only 1% of the predicted high risk credits are true high risk and 59% of the high risk credits are identified by this model. The F1 score is also quite low (0.01).

### IV. SMOTEENN Combination Sampling
![SMOTEENN](Resources/images/SMOTEENN.png)
* The balanced accuracy score is 63.8%.
* For high risk credits, the precision score is 1%, and the recall is 70%, which means only 1% of the predicted high risk credits are true high risk and 70% of the high risk credits are identified by this model. The F1 score is also quite low (0.02).

### V. Balanced Random Forest Classifier
![BRFensemble](Resources/images/BRFensemble.png)
* The balanced accuracy score is 78.8%.
* For high risk credits, the precision score is 4%, and the recall is 67%, which means 4% of the predicted high risk credits are true high risk and 67% of the high risk credits are identified by this model. The F1 score is slightly improved at 0.07.

### VI. Easy Ensemble Classifier
![EasyEnsembleClassifier](Resources/images/EasyEnsembleClassifer.png)
* The balanced accuracy score is 92.5%.
* For high risk credits, the precision score is 7%, and the recall is 91%, which means 7% of the predicted high risk credits are true high risk and 91% of the high risk credits are identified by this model. The F1 score is improved more at 0.14.

## Summary
In summary, the first four models are not good at predicating high risk credit because (1) Their balanced accuracy scores are all below 70%; (2) Their precision scores for high risk credit are very low (1-2%), incidating a large number of false high risk credits; (3) Their recall scores for high risk credit are also low (70% or below), which are indicative of a large number of false low risk credits. 

However, the two ensemble classifiers are much more effective catching high risk credits in comparison to the previous four models. Particularly, the Easy Ensemble Classifer performs the best with highest balanced accuracy score (92.5%), precision score (7%), recall (91%), and F1 score (0.14).  

Therefore, among the six machine leanring models, the Easy Ensemble Classifier is recommended to predict high risk credit.  
