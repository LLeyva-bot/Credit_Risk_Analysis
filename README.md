#Module_Seventeen_Credit_Risk_Analysis

## Project Overview
This porject is about applying machine learning to solve a real-world challenge: credit card risk. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we need to employ different techniques to train and evaluate models with unbalanced classes.
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Lastly, we evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Resources
 - Data Source: LoanStats_2019Q1.csv
 - Software: Python, Anaconda, Conda, Jupyter Notebook, Numpy, Sklearn, Imblearn

## Results

#### Credit Risk Sampling
Naive Random Oversampling Model:
![Fig1](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig1.png)
![Fig2](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig2.png)
 - Balanced Accuracy Score = 66%

SMOTE Oversampling Model:
![Fig3](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig3.png)
![Fig4](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig4.png)
 - Balanced Accuracy Score = 66%

Cluster Centroids Undersampling Model:
![Fig5](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig5.png)
![Fig6](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig6.png)
 - Balanced Accuracy Score = 54%

SMOTEENN Combination (Over and Under) Sampling Model:
![Fig7](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig7.png)
![Fig8](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig8.png)
 - Balanced Accuracy Score = 67%

#### Credit Risk Ensemble
Balanced Random Forest Classifier Model:
![Fig9](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig9.png)
![Fig10](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig10.png)
 - Balanced Accuracy Score = 78%

Easy Ensemble AdaBoost Classifier Model:
![Fig11](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig11.png)
![Fig12](https://github.com/LLeyva-bot/Credit_Risk_Analysis/blob/main/Images/Fig12.png)
 - Balanced Accuracy Score = 93%
