# Metabolic-Syndrome-Prediction
### This project is a data cleaning, wrangling, analysis, clustering, ML Modeling, and DL Modeling for a metabolic syndrome prediction
#### By: Mohammad Abu Ayyash (july 2024)
#### This project aims to help the medical persona understand the properties of metabolic syndrome that play crucial roles in predicting and further diagnosis a  metabolic syndrome case.
#### Data:
dtypes: float64(5), int64(6), object(4), 2401 entries,(total 14 columns),memory usage: 281.5+ KB
#### In this summary you'll find :

![1](https://github.com/user-attachments/assets/6f9b594a-128a-40b5-b380-325abcbb9173)

* as we notice the higher the triglycerides levels the higher the metabolic syndrome affection.


![2](https://github.com/user-attachments/assets/15acb2f4-8e9c-41cb-b13c-969248bf83b9)

* Also, we notice the higher the WaisCirc levels the higher the metabolic syndrome affection.


![download (12)](https://github.com/user-attachments/assets/a8cb99e9-63bc-48cc-89cc-479e21c4d42e)

* This is a general distribution based on sex wither its a male or female.

![download (13)](https://github.com/user-attachments/assets/fcd25eb0-feb7-401a-8636-555dcf35fd3a)

* This is a general distribution based on marital stauts.

![download (14)](https://github.com/user-attachments/assets/cd76b9c0-57ed-4bfa-adfd-bd840b0d5288)

* This is a general distribution based on race.

![download (15)](https://github.com/user-attachments/assets/b52f544d-a9d8-484b-aed2-661a881fc8e1)

* This is a general distribution based on age and sex.

#### Models used with their metrics:
Logistic Regression Model (Testing Set):

              precision    recall  f1-score   support

           0       0.84      0.92      0.88       395
           1       0.81      0.67      0.74       206

    accuracy                           0.83       601

Logistic Regression (SMOTE) Model (Testing Set):

              precision    recall  f1-score   support

           0       0.88      0.84      0.86       395
           1       0.72      0.78      0.75       206

    accuracy                           0.82       601

Logistic Regression (Gridsearch + SMOTE) Model (Testing Set):

              precision    recall  f1-score   support

           0       0.88      0.85      0.86       395
           1       0.73      0.78      0.75       206

    accuracy                           0.82       601

Logistic Regression (PCA) Model (Testing Set):

              precision    recall  f1-score   support

           0       0.84      0.91      0.87       395
           1       0.79      0.67      0.72       206

    accuracy                           0.83       601

Logistic Regression (K-Means) Model (Testing Set):

              precision    recall  f1-score   support

           0       0.88      0.87      0.87       395
           1       0.75      0.76      0.76       206

    accuracy                           0.83       601

Deep Learning Model (Testing Set):

              precision    recall  f1-score   support
              
           0       0.85      0.91      0.88       159
           1       0.79      0.70      0.74        82

    accuracy                           0.83       241


Deep Learning Model (Tunned) (Testing Set):

              precision    recall  f1-score   support
              
           0       0.95      0.40      0.56       159
           1       0.45      0.96      0.61        82

    accuracy                           0.59       241


Logistic Regression (Decision Threshold + Gridsearch + SMOTE) Model (Testing Set):

              precision    recall  f1-score   support

           0       0.90      0.81      0.85       395
           1       0.69      0.83      0.75       206

    accuracy                           0.82       601

#### Recommendations: 
The Final Model Chosen was the Logistic Regression (Decision Threshold + Gridsearch + SMOTE) Model, Using this model to make predictions about determination of metabolic syndrome would be reliable since the target we are trying to predict had the highest score percentage of accuracy for the test data which is 82%.

#### Much more useful information regarding this project is included in the ipynb.
