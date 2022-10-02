# Credit_Risk_Analysis
## Overview 
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results

### Naive Random Oversampling


<img width="1097" alt="Screen Shot 2022-10-01 at 1 56 16 PM" src="https://user-images.githubusercontent.com/104036750/193425605-17f0d85e-501d-4abb-8066-64f9af9a2b63.png">

* The balanced accuracy score is 66%.
* High_risk category: 1% precision and 68% recall score
* Low-risk category: 100% precision and 64% recall score

### SMOTE Oversampling


<img width="1101" alt="Screen Shot 2022-10-01 at 1 59 08 PM" src="https://user-images.githubusercontent.com/104036750/193425608-5185ff37-4fdd-45a9-9c2a-32d4bbf758ff.png">

* The balanced accuracy score is 66%.
* High_risk category: 1% precision and 63% recall score
* Low-risk category: 100% precision and 68% recall score

### Undersampling


<img width="1111" alt="Screen Shot 2022-10-01 at 1 59 27 PM" src="https://user-images.githubusercontent.com/104036750/193425610-d2faf7d1-003f-4201-af73-65a3f00efbe0.png">

* The balanced accuracy score is 66%.
* High_risk category: 1% precision and 68% recall score
* Low-risk category: 100% precision and 64% recall score

### Combination (Over and Under) Sampling


<img width="1095" alt="Screen Shot 2022-10-01 at 1 59 43 PM" src="https://user-images.githubusercontent.com/104036750/193425614-e889e1e7-0062-4dd4-8e3c-f6ffe2af1319.png">

* The balanced accuracy score is 64%.
* High_risk category: 1% precision and 72% recall score
* Low-risk category: 100% precision and 57% recall score

### Balanced Random Forest Classifier


<img width="1096" alt="Screen Shot 2022-10-01 at 2 42 31 PM" src="https://user-images.githubusercontent.com/104036750/193425752-6b835d38-cc6a-4ef8-b41c-cf83fe877170.png">

* The balanced accuracy score is 68%.
* High_risk category: 88% precision and 37% recall score
* Low-risk category: 100% precision and 100% recall score

### Easy Ensemble AdaBoost Classifier


<img width="1117" alt="Screen Shot 2022-10-01 at 2 42 45 PM" src="https://user-images.githubusercontent.com/104036750/193425754-b06b36a4-4cad-4dea-aa0a-1149f565713c.png">

* The balanced accuracy score is 93%.
* High_risk category: 9% precision and 92% recall score
* Low-risk category: 100% precision and 94% recall score

## Summary

Overall, the modules have weak precision when determining high credit risk. The Easy Ensenble AdaBoost Classifier had the best performance in detecting high risk credit but the precision is low, so a lot of low risk are being misrepresented as high risk. The best model for detecting low risk is the Random Forest Model, and overall, this model would be the best one to use for predicting credit risk. 
