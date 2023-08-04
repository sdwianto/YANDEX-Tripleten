## INTERCONNECT, a telecommunications operator, aims to forecast their client churn rate
#### <i>Sprint focus: Final Project. Helping ‘INTERCONECT’ a telecommunication operator company to predict ‘churn’ of their customer, and then if we know client have planning to stop company will give promotion offering and special package option </i>

Project Description: 
INTERCONNECT, a telecommunications operator, aims to forecast their client churn rate. When a client is planning to terminate services, they will be offered promotional codes and special package options. The marketing team has collected personal data of clients, including information about their selected data packages and contracts.
Reported Tasks: To meet Interconnect's needs in forecasting client churn rate, the following tasks were carried out:

Exploratory Data Analysis:
-	Checked for missing data, duplicates, and incorrect data types in the customer data (personal information, internet services, telephone packages, and contracts).
-	Handled missing numerical data by filling with the median value and performed encoding for categorical data.
-	Joined datasets, handled missing data after joining, and dropped unnecessary columns for model training.
-	Encountered challenges in dealing with data type issues, specifically for the contract column in TotalCharges, where the data type was initially an object (should be float).
-	Model training to predict client churn rate:
-	Performed hyperparameter tuning for the imbalanced target data by adjusting class weights, upsampling, and downsampling.
-	Initially tried Logistic Regression, Decision Tree, Random Forest, and LGBM models but found their AUC-ROC below the desired threshold (0.85).
-	Added XGBoost and after several tuning iterations, achieved a final AUC-ROC above 0.85.

Key steps to complete the task include understanding Interconnect's goal, studying client data, preparing data for prediction, and tuning model parameters to achieve the desired evaluation metrics.

Testing the Selected Model on Test Data: After multiple experiments with different learning models, the most optimal model for predicting client churn rate was XGBoost, with tuned parameters:
-	n_estimators=90
-	use_label_encoder=False
-	eval_metric='mlogloss'
-	random_state=1
-	objective='binary:logistic'
-	tree_method='hist'
-	eta=0.1
-	max_depth=3

Results:
-	Train F1 score: 0.6546290216677609
-	Test F1 score: 0.6423357664233577
-	AUC-ROC: 0.8674038214691753

The XGBoost model showed the best performance in predicting client churn rate for Interconnect.
