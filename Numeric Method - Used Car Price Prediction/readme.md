## Used Car Price Prediction 
#### <i>Sprint focus: Numeric Method, Linear Regression, Gradient Descent, Neural Network, Gradient Boosting, Gradient Boosting Library (XGBoost, LightGBM, CatBoost) </i>

Summary: 
The project involves the development of an application for Rusty Bargain, a used car trading company, to attract new buyers by providing quick and accurate market values for their cars. The model's performance was evaluated based on prediction quality, prediction speed, and training time.

The performance of different models is as follows:
1.	Linear Regression:
-	Training time: 239 ms
-	Prediction time: 40.6 ms
-	RMSE scores: Train - 3122.71756, Valid - 3107.08173, Test - 3104.9996
2.	Decision Tree:
-	Training time: 1.97 s
-	Prediction time: 115 ms
-	RMSE scores: Train - 860.20808, Valid - 2567.09035, Test - 2590.21463
3.	Random Forest:
-	Training time: 26.7 s
-	Prediction time: 1.99 s
-	RMSE scores: Train - 2306.24578, Valid - 2342.71906, Test - 2341.61124
4.	LGBM:
-	Training time: 1.16 s
-	Prediction time: 432 ms
-	RMSE scores: Train - 2382.51669, Valid - 2394.83998, Test - 2390.46661

Conclusion:
-	The Random Forest model provides the best prediction quality.
-	Linear Regression exhibits the fastest prediction speed.
-	The shortest training time is achieved using Linear Regression.
-	The recommendation for Rusty Bargain is to use the Decision Tree model, as it offers a balanced combination of prediction accuracy and speed.

Note: The summary provided is based on the given performance metrics for each model. However, it is important to consider other factors, such as interpretability and generalization ability, when choosing the final model for deployment.
