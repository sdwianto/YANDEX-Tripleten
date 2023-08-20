## The insurance company "SURE TOMORROW" aims to address several issues using machine learning
#### <i>Sprint focus: Linear Algebra, vector, Euclides distance, Manhattan distance, K-NN, Transpose metrics, Invers Metrics</i>

Summary:
The insurance company "SURE TOMORROW" aims to address several issues using machine learning. The evaluation of the feasibility of these tasks resulted in the following findings:

Task 1: Finding Similar Clients
-	Non-scaled data affects the kNN algorithm, resulting in differences in data point distances compared to scaled data.
-	Both the Euclidean and Manhattan distance metrics show similar patterns with the same index order, but the distances differ.
-	Classification based on kNN with non-scaled data yielded an F1 score of 0.27, while scaled data achieved a significantly higher score of 0.92.
-	The classification model with scaling demonstrated better precision and recall compared to the dummy prediction model.
  
Task 2: Predicting Insurance Claims
-	The kNN-based classification model outperformed the dummy model for both scaled and non-scaled data.
-	The dummy model's predictions were not superior to the kNN model for claim prediction.
  
Task 3: Predicting Potential Amount of Insurance Claims
-	Using linear regression with the insurance benefit as the target, the model achieved an RMSE of 0.34, indicating reasonably good accuracy.
-	The R-squared score of 0.66 suggests that the linear regression model is relatively suitable for predicting insurance benefits.

Task 4: Protecting Client Data
-	Data transformation operations involving matrix inversion and transposition led to differences in some values, primarily due to non-zero scalar values (k) in the matrix inversion.
-	Transformation of data such as client age or income resulted in randomness, loss of structured information, and mismatched values, making it difficult to predict the transformed data.

Conclusion: The evaluation highlighted the importance of scaling data for kNN algorithms and the impact of data transformation on prediction accuracy. The kNN-based classification model with scaling outperformed the dummy model, and the linear regression model showed reasonably good accuracy for predicting insurance benefits. Ensuring data protection without compromising model quality is essential for "Sure Tomorrow" to effectively utilize machine learning for addressing their business challenges.
