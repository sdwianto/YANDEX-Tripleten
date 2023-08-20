To meet Interconnect's requirement for predicting customer churn rate, the following steps were taken:

Exploratory Data Analysis:
The customer data from Interconnect, including personal information, internet services, phone packages, and client contracts, underwent various checks and adjustments. These included handling missing values (NaN), identifying duplicates, adjusting data types, imputing numerical NaN values with medians, encoding categorical data, joining datasets, filling missing values post-joining, and dropping unnecessary columns for model training.

Challenges arose while handling contract data, particularly the 'TotalCharges' column, which initially had an object data type that needed conversion to float. Additionally, proper imputation of missing values in categorical data was achieved using the mode (initially median was used for NaN values).

Model Training for Predicting Customer Churn:
Hyperparameter tuning was essential due to the imbalanced target data. Techniques used involved:

Class weight adjustment
Upsampling data
Downsampling data
Initially, only four models were employed for predicting churn: Logistic Regression, Decision Tree, Random Forest, and LGBM. However, their performance fell below the desired threshold (AUC-ROC below 0.85). As a result, XGBoost was introduced and after multiple rounds of parameter tuning, a final AUC-ROC above 0.85 was achieved.

Key Steps in Task Completion:
Understanding Interconnect's goals, studying client data, data preparation for prediction, and model parameter tuning were pivotal in achieving the desired performance metrics.

Testing the Chosen Model on Test Data:
After conducting diverse trials with various learning models, XGBoost emerged as the most optimal model for predicting Interconnect's customer churn rate. The refined parameter settings included:

n_estimators=90,
use_label_encoder=False,
eval_metric='mlogloss',
random_state=1,
objective='binary:logistic',
tree_method='hist',
eta=0.1,
max_depth=3
The results were as follows:

Train F1 score: 0.6546290216677609
Test F1 score: 0.6423357664233577
AUC-ROC: 0.8674038214691753
