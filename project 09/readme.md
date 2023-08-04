## OILYGIANT wants to find suitable locations for drilling new oil wells
#### <i>Sprint focus: Machine Learning in Business Application, Income, Sales, Margin, Profit, Funneling, A/B Testing, Pipeline, Bootstrapping, Labeling, Data Leakage, Cross-Validation </i>


Project Summary:
The project involves working for an oil mining company named OILYGIANT and aims to find suitable locations for drilling new oil wells. The steps to select the location include collecting parameters like oil quality and oil reserve volume, creating a predictive model for oil reserve volume, selecting the oil well with the highest estimated value, and finally choosing the region with the highest total profit from the selected 

oil wells. The analysis is based on sample oil data from three regions and involves using bootstrapping techniques to assess potential profits and risks.

Findings:
-	Region 2 has the highest mean value of well reserve prediction, but it also has the highest RMSE value, indicating lower prediction accuracy.
-	Region 1 has the smallest mean value of well reserve prediction and the lowest RMSE value, indicating better prediction accuracy.
-	Region 0 has relatively high mean values of well reserve prediction and RMSE.

Insights:
-	Despite having the best prediction accuracy, Region 1 has the lowest predicted mean value of well reserve.
-	The minimum well reserve required for profitability is 111 barrels.
-	Region 0 has the highest well reserve prediction.

More Findings:
-	Region 0 has the highest number of top-ranked wells with 31,102 barrels.

Recommendations:
-	The company should explore and drill new wells in region 0, as it has the top 200 predicted wells with the highest reserve and the highest predicted and target profit.
-	Alternatively, the company should explore and drill new wells in region 1, as it has the highest mean profit calculation and a low risk of losses.

Conclusion:
Based on RMSE calculations and bootstrapping techniques with 1000 samples, Region 1 is identified as the best region to develop new wells. Both profit calculations, using prediction base and target base methods, show that Region 1 offers the highest profit values with a slightly lower risk of losses (less than 1%). Therefore, it is recommended for OILYGIANT to explore and drill new wells in region 1 to maximize profits and minimize risks.
