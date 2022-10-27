# Credit_Risk_Analysis

## Overview
The purpose of this analysis was to employ different machine learning techniques to train and evaluate models with unbalanced classes. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. This analysis reviews loan data in relation to lending risk.

Deliverable 1: Use Resampling Models to Predict Credit Risk

Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk

Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk

## Resources

  -Data Source: LoanStats_2019Q1.csv
  
  -Software: Python, Jupyter Notebook, imbalanced-learn, scikit-learn
  
## Analysis and Results of Data

There weree six different machine learning methods used to analyze loan data from LendingClub, a popular lending services company. Each method is listed below with the typical drawback of that method (no method is perfect) and the results of each analysis.

**1. Oversampling**

Oversampling is prone to overfitting. Overfitting often fails to predict future data reliably because results correspond too closely or exactly to the training and test sets.

- Accuracy Score: 65% 
- 
![D1_Accuracy_Score](https://user-images.githubusercontent.com/108022219/198174332-b61af170-8372-442a-9a78-5b282b223f4b.png)

- Confusion Matrix
- 
![D1_confusion_matrix](https://user-images.githubusercontent.com/108022219/198174335-c93e1cc0-26e7-4980-87e0-145397f9ece6.png)

-Classification Report

![D1_Classification_report](https://user-images.githubusercontent.com/108022219/198174334-dfa44d61-7e76-40ae-8fec-c6ab1883ae58.png)

**2. Oversampling with SMOTE (Synthetic Minority Oversampling Technique)**

SMOTE is still oversampling and is still prone to overfitting. Using the synthetic method can help to overcome class imbalances and lessen the exactness of outcome dependency on minority classes.

-Accuracy Score:  66%
-Confusion Matrix and Classification Report

![D2_Smote](https://user-images.githubusercontent.com/108022219/198175281-c20db79a-a8f1-40df-a4df-3f076c967208.png)

**3. Combination (Over+Under) Sampling with SMOTEENN (Edited Nearest Neighbors)**

Using SMOTE to oversample via synthetic methods to help overcome class imbalances -- and then also ENN and choose more relevant minority classes may not make any relevant gains in predictive accuracy but it may provied quality comparison value.

-Accuracy Score:  65%
-Confusion Matrix and Classification Report

![D2_Over_Under_Sampling](https://user-images.githubusercontent.com/108022219/198175278-e9c6f8d8-2a4a-4ea6-95b6-01446a5831db.png)

**4. UnderSampling**

Undersampling tries to balance data by keeping all minority classes. Undersampling can often lower accuracy for datasets having minority classes not closely correlated to the majority classes

-Accuracy Score: 54%
-Confusion Matrix and Classification Report

![D2_Undersampling](https://user-images.githubusercontent.com/108022219/198175615-aab4b615-9987-4264-a4f8-45dfa99a23b4.png)

**5. Ensemble Learning with Random Forest**

Ensemble learning methods use combined methods to predict and are best used when performance on a predictive modeling project is the most important outcome. The reasoning for the higher performance is not always easy to decipher though, and depending on the size of the dataset, ensemble modeling can end up using far more resources.

-Accuracy Score: 79%
-Confusion Matrix and Classification Report

![D3_BalancedRandomForest](https://user-images.githubusercontent.com/108022219/198176930-9844c8f2-e8bc-4525-808a-a30bfc73e41a.png)

**6. Ensemble Learning with Easy Ensemble**

Ensemble learning methods use combined methods to predict and are best used when performance on a predictive modeling project is the most important outcome. The reasoning for the higher performance is not always easy to decipher though, and depending on the size of the dataset, ensemble modeling can end up using far more resources.

-Accuracy Score: 93%
-Confusion Matrix and Classification Report

![D3_Ensemble](https://user-images.githubusercontent.com/108022219/198178279-65f2cb2b-255f-4287-b5f7-013acb6122f0.png)


## Summary 
The final Easy Ensemble learning method produed the highest accuracy score (93%) and the highest F1 score, as well as great precision and sensitivity scores, it would appear to be the best method for predicting risk for this data.

