## Develop a model for MEGALINE mobile operator to analyze customer behavior and recommend one of their two newest plans
#### <i>Sprint focus: Machine Learning, Classification and Regression, Accuracy, Evaluation Metric, Underfitting and Overfitting, Decision Tree, Hyperparameter Tunning, Random Forrest, Logistic Regression </i>

Summary:
The project aims to develop a model for MEGALINE mobile operator to analyze customer behavior and recommend one of their two newest plans, Smart or Ultra, with a minimum accuracy of 0.75. 

The findings from the MEGALINE customer dataset are as follows:
- The majority of customers (70%) use the Smart plan package. 
- The dataset was divided into training, validation, and testing sets, and the model did not show signs of overfitting. 
- Decision Tree and Random Forest regression were used to improve model accuracy. 
- Random Forest regression with max_depth_best = 9 and n_estimators_best = 200 achieved the highest testing accuracy score of 80.87%.

Insights: 
- Unbalanced datasets can lead to improper models and lower accuracy scores.

Recommendation: 
- The recommended model for MEGALINE is Random Forest regression with max_depth_best = 9 and n_estimators_best = 200 to understand customer behavior and plan package preferences effectively.
