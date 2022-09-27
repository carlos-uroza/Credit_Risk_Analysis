# Module 17 Challenge - Credit_Risk_Analysis

## Overview of the Project

### Purpose
The purpose of this project is to correct the class imbalance found in our credit card dataset to accurately solve a credit risk classification problem. Our program uses a variety of different resampling techniques from the imbalanced-learn and scikit-learn libraries to build and evaluate two seperate Ensemble classifiers.

## Results

### Deliverable 1 - Use Resampling Models to Predict Credit Risk

- Naive Random Oversampling

This model had a balanced accuracy score of 65.15%, a total precision score of 0.99, and a total recall score of 0.68

![Naive Random Oversampling](https://user-images.githubusercontent.com/103288980/192436788-f4d55b47-1e0f-4511-a456-2366aee7cd04.PNG)

- SMOTE Oversampling

This model had a balanced accuracy score of 62.41%, a total precision score of 0.99, and a total recall score of 0.66

![SMOTE Oversampling](https://user-images.githubusercontent.com/103288980/192436804-7a39624b-58f7-4f04-a5f5-c577ef87e79d.PNG)

- Undersampling

This model had a balanced accuracy score of 51.59%, a total precision score of 0.99, and a total recall score of 0.44

![Undersampling](https://user-images.githubusercontent.com/103288980/192436821-5751833c-e38c-444b-9918-1633fd44de7d.PNG)

### Deliverable 2 - Use the SMOTEENN Algorithm to Predict Credit Risk

- Combination (Over and Under) Sampling

This model had a balanced accuracy score of 64.65%, a total precision score of 0.99, and a total recall score of 0.58

![SMOTEENN](https://user-images.githubusercontent.com/103288980/192436841-9a27af34-b37a-4b45-a661-1fd98732533a.PNG)

### Deliverable 3 - Use Ensemble Classifiers to Predict Credit Risk

- Balanced Random Forest Classifier

This model had a balanced accuracy score of 78.77%, a total precision score of 0.99, and a total recall score of 0.91

![Balanced Random Forest Classifier](https://user-images.githubusercontent.com/103288980/192436852-0f030c97-6ccc-4cd9-83fa-9ef13efbd236.PNG)

- Easy Ensemble AdaBoost Classifier

This model had a balanced accuracy score of 92.54%, a total precision score of 0.99, and a total recall score of 0.94

![Easy Ensemble AdaBoost Classifier](https://user-images.githubusercontent.com/103288980/192436866-bcba2c91-a63d-45f4-976e-011146012187.PNG)

## Summary

### Recommendations
In summary, applying the resampling methods to our initial Logist Regression model did not significantly improve the accuracy of the model. However, applying the resampling methods to our Ensemble Classifier models resulted in a significant increase to our overall accuracy. 
It is our recommendation that our customer use the Easy Ensemble AdaBoosted Classifier model to predict credit risk of unbalanced data as this model holds the highest balanced accuracy score and has a high precision score for low_risk. However, the Lender is advised this model is an effective classifier for low_risk loans and shows significant False Negative errors. This is a situation where the Lender may reject customers whom should be eligible, potentially missing the opportunity cost of revenues and profits. However, Lender can be assured the model catches all actual high risk applications.
