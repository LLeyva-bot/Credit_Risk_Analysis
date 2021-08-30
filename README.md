#Module_Seventeen_Credit_Risk_Analysis

## Project Overview
This project is about applying machine learning to solve a real-world challenge: credit card risk. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we need to employ different techniques to train and evaluate models with unbalanced classes.
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we oversample the data using the RandomOverSampler and SMOTE algorithms, and under sample the data using the ClusterCentroids algorithm. Then, we use a combinatorial approach of over- and under sampling using the SMOTEENN algorithm. Next, we compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Lastly, we evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Resources
 - Data Source: LoanStats_2019Q1.csv
 - Software: Python, Anaconda, Conda, Jupyter Notebook, Numpy, Sklearn, Imblearn

## Results

### Credit Risk Sampling
#### Naive Random Oversampling Model:
 - Balanced Accuracy Score = 66%

![Fig1](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig1.png)
![Fig2](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig2.png)

 #### SMOTE Oversampling Model:
 - Balanced Accuracy Score = 66%

![Fig3](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig3.png)
![Fig4](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig4.png)


#### Cluster Centroids Under Sampling Model:
 - Balanced Accuracy Score = 54%

![Fig5](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig5.png)
![Fig6](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig6.png)


#### SMOTEENN Combination (Over and Under) Sampling Model:
 - Balanced Accuracy Score = 67%

![Fig7](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig7.png)
![Fig8](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig8.png)


### Credit Risk Ensemble
#### Balanced Random Forest Classifier Model:
 - Balanced Accuracy Score = 78%

![Fig9](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig9.png)
![Fig10](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig10.png)


#### Easy Ensemble AdaBoost Classifier Model:
 - Balanced Accuracy Score = 93%

![Fig11](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig11.png)
![Fig12](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig12.png)

## Summary
The Easy Ensemble AdaBoost Classifier model has the highest balanced accuracy score at 93%.  The Balanced Random Forest Classifier model has the next highest accuracy score at 78%.  Overall, the Credit Risk Ensemble models displayed more sensitivity toward high risk credit scores which made them more accurate.  Although, 93% may appear as a high accuracy score, all models need improvement.  All models need to improve to better detect low risk credit scores..  After evaluating all models, we found low risk credit scores are being falsely detected as high risk which would penalize the bank's credit strategy and impact their revenue by missing those business opportunities.
