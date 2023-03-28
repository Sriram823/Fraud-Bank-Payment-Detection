# Fraud-Bank-Payment-Detection
Applying Machine Learning Models to detect Fraudulent Bank payments on a synthetically generated dataset.

We detect the fraudulent transactions from the Banksim dataset. This synthetically generated dataset consists of payments from various customers made in different time periods and with different amounts.

Here what we'll do in this kernel:
-> Exploratory Data Analysis (EDA)
-> Data Preprocessing
-> Oversampling with SMOTE
-> K-Neighbours Classifier
-> Random Forest Classifier
-> XGBoost Classifier


Classification Report for K-Nearest Neighbours: 

         |class|     precision |   recall | f1-score  | support|
         |------| -----------|----------|---------|---------|
         |  0 |      1.00  |    0.98  |    0.99  |  176233|
          | 1  |     0.98  |    1.00 |     0.99|    176233|
           
    accuracy                           0.99    352466
   macro avg       0.99      0.99      0.99    352466
weighted avg       0.99      0.99      0.99    352466

Confusion Matrix of K-Nearest Neighbours: 
 [[171999   4234]
 [   362 175871]]
 
Classification Report for Random Forest Classifier: 
               precision    recall  f1-score   support
           0       0.99      0.97      0.98    176233
           1       0.97      0.99      0.98    176233
    accuracy                           0.98    352466
   macro avg       0.98      0.98      0.98    352466
weighted avg       0.98      0.98      0.98    352466

Confusion Matrix of Random Forest Classifier: 
 [[170106   6127]
 [  1079 175154]]
 
 
Classification Report for XGBoost: 

               precision    recall  f1-score   support
           0       1.00      0.99      0.99    176233
           1       0.99      1.00      0.99    176233
    accuracy                           0.99    352466
   macro avg       0.99      0.99      0.99    352466
weighted avg       0.99      0.99      0.99    352466

Confusion Matriz of Xboost: 
 [[174033   2200]
 [   775 175458]]


Original Paper:

Lopez-Rojas, Edgar Alonso ; Axelsson, Stefan Banksim: A bank payments simulator for fraud detection research Inproceedings 26th European Modeling and Simulation Symposium, EMSS 2014, Bordeaux, France, pp. 144–152, Dime University of Genoa, 2014, ISBN: 9788897999324. https://www.researchgate.net/publication/265736405_BankSim_A_Bank_Payment_Simulation_for_Fraud_Detection_Research
