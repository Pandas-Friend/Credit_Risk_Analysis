# Credit_Risk_Analysis
### Overview
The purpose of this project was to apply machine learning to solve a real-world challenge: credit card risk. I employed different techniques to train and evaluate models with unbalanced classes. I used imbalance-learn and scikit-learn libraries to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and under sampled the data using the ClusterCentroids algorithm. Then I used a combinatorial approach of over and under sampling using the SMOTEENN algorithm. Next I compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.
### Results
Oversampling
Naïve Random Oversampling

![pic1](Resources/pic1.png)

SMOTE Oversampling

![pic2](Resources/pic2.png)

Under Sampling
Cluster Centroids Algorithm

![pic3](Resources/pic3.png)

Combination (Over and Under) Sampling
SMOTEENN

![pic4](Resources/pic4.png)

Ensemble Learners
Balanced Random Forest Classifier

![pic5](Resources/pic5.png)

Easy Ensemble AdaBoost Classifier

![pic6](Resources/pic6.png)

### Summary
All of our models show a very weak precision when determining high risk credit. The ensemble models showed improvement over the other 4, as the recall improved quite a bit with these models. The EasyEnsembleClassifier model was the best one with a recall of 84 percent for high risk and 95 percent for low risk. But with a precision of 8 percent for high risk a lot of low risk credit is flagged as high risk that shouldn’t be.
