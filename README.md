# Credit_Risk_Analysis
Module 17 Challenge 

# Overview 
Below you will find a reveiw of different machine learning models that are being used to try and predict credit risk. We unfortunately began with a very unbalanced dataset. The data is unbalanced because more good loans are given than risky ones or loans where the borrower could be called in defult. Using resampling algorithms and two ensemble classifiers we hope to work with this tricky data and avoid high risk borrowers. 

# Results 
## Oversampling 
* Balanced Accuracy Score: 0.64
* Precision Score: High Class 0.01, Low Class 1.0
* F1 Score: High Class 0.02, Low Class 0.79
* Recall Score: High Class 0.62, Low Class 0.65
![Oversampling ](/Resources/oversampling.png)

## SMOTE 
* Balanced Accuracy Score: 0.63
* Precision Score: High Class 0.01, Low Class 1.0
* F1 Score: High Class 0.02, Low Class 0.78
* Recall Score: High Class 0.62, Low Class 0.64
![SMOTE](/Resources/smote.png)

## Undersampling
* Balanced Accuracy Score: 0.52
* Precision Score: High Class 0.01, Low Class 1.0
* F1 Score: High Class 0.01, Low Class 0.60
* Recall Score: High Class 0.60, Low Class 0.43
![Undersampling](/Resources/undersampling.png)

## SMOTEENN
* Balanced Accuracy Score: 0.64
* Precision Score: High Class 0.01, Low Class 1.0
* F1 Score: High Class 0.02, Low Class 0.73
* Recall Score: High Class 0.70, Low Class 0.57
![SMOTEEN](/Resources/smoteenn.png)

## Balanced Random Forest Classifier
* Balanced Accuracy Score: 0.79
* Precision Score: High Class 0.04, Low Class 1.0
* F1 Score: High Class 0.07, Low Class 0.95
* Recall Score: High Class 0.67, Low Class 0.91
![Balanced Forest](/Resources/balancedforest.png)

## Easy Ensemble AdaBoost Classifier
* Balanced Accuracy Score: 0.92
* Precision Score: High Class 0.07, Low Class 1.0
* F1 Score: High Class 0.14, Low Class 0.97
* Recall Score: High Class 0.91, Low Class 0.94
![Adaboost](/Resources/adaboost.png) 

# Summary 
When comparing the results of the first four models to the last two you can easily see that utilizing ensemble learning imporoved the machine learning models. Particularily the Easy Ensemble AdaBoost Classifier is the strongest. To prove this first look at the accuracy scores, which compared the actual values from the test set against the models predicted values. In the Adaboost model 92% of predictions of risk are correct. Additionally when looking at the precision, F1 and recall scores we should care about precision the most, because we want to ensure we are correct about the risk eligibility of the loan applicant.The Adaboost model gives us the highest precision score in the high class, 0.07. Recall scores would asist us in evaluating when we know someone was at risk of defulting on thier loan, what would the chance be they actually defult? As we are working with a binary outcomes, a loan is risky or not, we  would be most concerned of the false possitives in our model. Or the high risk loan applicants accidently labeled as low risk.  

