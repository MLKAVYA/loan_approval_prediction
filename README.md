#Loan Approval Prediction Using Machine Learning

This is a supervised machine learning classification task to predict whether a loan will be approved('Loan_status') based on customer details.
Two powerful ensemble models-**Gradient Boosting** and **CatBoost**-were trained and evaluated for comparison.
-----
## Dataset
The dataset used contains the following features:
-Gender,Married,Dependents,Education,Self_Employed,ApplicantIncome,LoanAmount,Credict_Hitory,Property_Area,CoApplicantIncome
-Target:'Loan_Status'(Yes/No)
-----
##Exploratory Data Analysis(EDA)
 Before training the models,EDA was performed to understand patterns,and relationship between features.
 Visuals like countplot and histplot is used to understand the relationship between target and features.
-----
## Problem Statment
Predict whether a loan will be approved based on customer details provided by the bank.This can help the institution in automating the approval
process and assessing risk.
-----
##Preprocessing Steps
-Handled missing values -Categorical features encoded -Normalized numerical features(where needed) -Split dataset into training and test sets.
-----
## Models Used
 1.**Gradient Boosting Classifier**
 2.**CatBoost Classifier**
Both models were trained on the same preprocessed dataset for fair comparison.
-----
## Evaluation Metrics
### Accuracy
 1.**Gradient Boosting Classifier** :0.7662
 2.**CatBoost Classifier** : 0.818
### Confusion Matrix
 1.**Gradient Boosting Classifier** :[[ 7 14]
                                     [ 4 52]]
  
 2.**CatBoost Classifier** :[[ 7 14]
                             [ 4 52]]
### Classification Report
 1.**Gradient Boosting Classifier**:  
                  precision    recall  f1-score   support

           0       0.64      0.33      0.44        21
           1       0.79      0.93      0.85        56

    accuracy                           0.77        77
   macro avg       0.71      0.63      0.64        77
weighted avg       0.75      0.77      0.74        77

2.**CatBoost Classifier**:
                 precision    recall  f1-score   support

           0       1.00      0.33      0.50        21
           1       0.80      1.00      0.89        56

    accuracy                           0.82        77
   macro avg       0.90      0.67      0.69        77
weighted avg       0.85      0.82      0.78        77
-----

## Prediction Differences Between Models
 Though both models were trained on the same data,they sometimes predicted differently for the same test samples.this can happens due to:
-Differences in how each model handles categorical features.
-internal strategies.
-Overfitting/underfitting of one model compared to the other.
**Observation:**While CatBoost has a higher overall accuracy,Gradient Boosting had slightly better precision for the 'No'class.This highlights
the importance of model comparison based on the bussiness goal(e.g:minimizing false approvals  and maximaizing loan distribution).
----- 
**Conclusion**:
->CatBoost outperformed Gradient Boosting in accuracy and recall.
->Ensemble models provide robust performance for real-world classifiation problem like this.
->selecting a appropriate model is very important.
-----
*Author*
 KAVYA M
 B.sc physics Graduate|Aspring Datascientist








