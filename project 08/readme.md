## Customer Prediction for BETA Bank
#### <i>Sprint focus: Supervised Learning, features importance, One-Hot-Encoding, Sanity Check, Imbalance Data, Recall, Precision, F1 Score, Up sampling, Down sampling, AUC-ROC, MSE, MAE </i>

Project Summary:
BETA Bank is experiencing a decline in its customer base every month. The bank has realized that it is more cost-effective to retain its existing loyal customers rather than acquiring new ones. The goal of the project is to predict whether a customer is likely to leave the bank soon or not. The main objectives are to develop a model with the maximum F1 score and ensure that the minimum F1 score on the testing dataset is 0.59. Additionally, the AUC-ROC metric will be calculated and compared with the F1 score.

Conclusion:
The analysis of the customer data led to the following conclusions:
-	Customer attrition: The number of customers leaving Beta Bank has been decreasing, resulting in a decline in the customer base.
-	Importance of retaining loyal customers: The analysis revealed that retaining loyal old customers is more cost-effective than acquiring new ones.
-	Best model for prediction: The best model for predicting customer churn was developed using Random Forest Regression with n_estimators = 100 and down sampling the data.
-	Model performance: The chosen model achieved an F1 score of 0.6438746438746439 and an AUC-ROC of 0.8733063525249727.

Recommendation:
Based on the results of the analysis, it is recommended that Beta Bank's employees focus on increasing engagement with their existing loyal customers to prevent further customer churn and maintain the customer base. This could involve personalized services, loyalty programs, and other initiatives to enhance customer satisfaction and loyalty. By doing so, the bank can protect its customer base and stabilize its business operations.
