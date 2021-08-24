# Credit Risk Analysis

## **Overview**

This project is a mock scenario where Lending Club, a peer-to-peer lending services company, wants to use machine learning to predict credit risk. Management believes it&#39;s a great way to provide a quicker and more reliable loan experience. It will also lead to more accurate identification of good candidates for loans which will lead to lower default rates. Therefore, they hire a data analyst to implement their plan.

Using the credit card credit dataset, **Python** was used to build and evaluate several machine learning models to predict credit risk. Being able to predict credit risk with machine learning algorithms can help banks and financial institutions

Different techniques were deployed to train and evaluate models with unbalanced classes, using to **imbalanced-learn**  and  **scikit-learn**  libraries. Oversample was done using the  **RandomOverSampler**  and  **SMOTE**  algorithms, and undersampling using the  **ClusterCentroids**  algorithm. Then, combinatorial approach of over- and undersampling was done using the  **SMOTEENN**  algorithm. Later on, we compared the two new machine learning models that reduce bias using,  **BalancedRandomForestClassifier**  and  **EasyEnsembleClassifier**.

## **Results**

### 1- Oversampling – Naive Random Oversampling
 
![](images/Naive.PNG)

### 2- Oversampling – SMOTE

![](images/SMOTE.PNG)

### 3- Undersampling – ClusterCentroids

![](images/Undersampling.PNG)

### 4- Combination (Over and Under) Sampling – SMOTEENN

![](images/Combination.PNG)

### 5- Ensemble Learners – Balanced Random Forest Classifier
 
![](images/Balanced.PNG)

### 6- Ensemble Learners – Easy Ensemble AdaBoost Classifier
 
![](images/AdaBoost.PNG)

## **Analysis of Results and Summary**

Looking at the performance of all six models above it’s hard to recommend any of them to be used for predicting credit risk. All of them had a 100% precision for low-risk, and lower than 8% of precision for high-risk. 

For oversampling model, naïve, the precision score is 0.01, sensitivity(recall) is 0.69 and F1 score is 0.02. 
For oversampling model, SMOTE , the precision score is 0.01, sensitivity is 0.68, and F1 score is 0.02, which make both of them very similar. 
Almost same results appeared with undersampling model. The precision score is 0.01, sensitivity is 0.69, and F1 score is 0.01. While SMOTEENN model also had 0.01 for precision score, sensitivity is 0.71, and F1 score is 0.02.

The random forest classifier had 0.03 for precision score, sensitivity is 0.70, and F1 score is 0.06.
And AdaBoost Classifier has, 0.09 for precision score, sensitivity is 0.92, and F1 score is 0.16.
Even though, AdaBoost Classifier has a better result, having the precision score and sensitivity than the rest, it still not reliable enough to be used for predicting credit risk. 


