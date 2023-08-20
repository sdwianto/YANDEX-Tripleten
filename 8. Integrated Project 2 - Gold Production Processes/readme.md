## Develop a model to predict the recovery of gold during the purification processes in ZYFRA
#### <i>Sprint focus: Integrated Project 2, Helping Zyfra to develop model for Gold Mining industry to have efficient production processes. </i>

Project Summary:
The project involves working with data from Zyfra company related to gold purification processes. The data is stored in three files: gold_recovery_train.csv (training dataset), gold_recovery_test.csv (test dataset), and gold_recovery_full.csv (source dataset). The data is indexed based on the date and time of acquisition, and some parameters may not be available in both the training and test sets. The goal is to create a model to predict the recovery of gold during the purification processes.

Findings:
-	The purification of gold follows a sequential process, starting from rougher input, rougher output, primary cleaner, and becoming the final output.
-	The concentration of gold increases at each stage of purification.
-	The purification of silver also follows a sequential process, and the concentration of silver increases at each stage.
-	The purification of lead involves different stages, and the highest concentration of lead is found in the rougher output stage.



-	Some features, such as 'rougher.output.recovery' and 'final.output.recovery,' have missing values in both the train and test datasets, which were filled with median values.
-	The models were evaluated using cross-validation, and RandomForest regression with depth 3 and n_estimators = 50 was found to be the best model for predicting the recovery of gold.

Conclusion:
Based on the analysis of the data and model evaluations, the project successfully developed a model to predict the recovery of gold during the purification processes. The selected RandomForest regression model with specific hyperparameters achieved better performance than the baseline values and provided reliable predictions. This model can be used to optimize gold purification processes and improve overall efficiency in the gold mining industry.
