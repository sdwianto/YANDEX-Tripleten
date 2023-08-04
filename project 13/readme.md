## Taxi order prediction
#### <i>Sprint focus: Time Series, Resampling, Rolling Mean / Moving Average, Trend, Seasonality, Stationary, Time series differences, Time Series Forecasting, Sanity Check </i>

Summary: 
The project involves the taxi company Sweet Lift, which has collected historical data on taxi orders at the airport. To attract more drivers during peak hours, the company aims to predict the number of taxi orders for the next hour. The task is to create a model capable of making such predictions, with the RMSE metric on the test set not exceeding 48.

Conclusion: After analyzing historical taxi order data from Sweet Lift, considering a one-hour sampling, and using 90% of the data for training and 10% for testing, the following results were obtained:
1. RMSE with traditional analysis methods:
-	ARIMA method: 53.5
-	Holt-Winter exponential smoothing: 79.7
-	Single exponential smoothing: 62.7
2.	RMSE with machine learning methods:
-	Linear Regression: 51.21672
-	Decision Tree (depth 6): 55.66404
-	Random Forest (no depth specified): 46.01577
-	LGBM: 50.6

Based on these results, the best prediction for the number of taxi orders in the next hour is achieved using the Random Forest model, with the lowest RMSE value of 46.0157.
