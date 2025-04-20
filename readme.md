Used Vehicle Price Analysis & Strategy Report

Audience: Used Car Dealerships

Goal: Identify factors driving used car prices and provide recommendations
________________________________________________________________________
1. Project Summary
We analyzed over 426,000 vehicle listings to determine what factors most influence price and how dealers can make smarter purchase and resale decisions. Two regression models were used:
	•	Linear Regression
	•	Ridge Regression (to try to avoid overfitting)
________________________________________________________________________
2. Data Preparation
	•	Removed entries with missing or unrealistic values (e.g., price < $1,000 or year < 1980)
	•	Created features such as follows:
		o	Car Age = 2025 − Year
		o	Price per Mile = Price / Odometer
	•	Focused on more important vehicle attributes such as make, year, mileage, condition, fuel type, transmission, etc.
________________________________________________________________________
3. Model Performance Comparison
Metric	Linear Regression	Ridge Regression
MAE	$5,717.50	$5,746.00
RMSE	$8,547.24	$8,591.68
R² Score	0.66	0.66

| Metric         | Linear Regression                      | Ridge Regression  |
|-----------------|----------------------------------------------|-----------------------------|
| MAE                | $5,717.50                                         | $5,746.00          |
| RMSE             | $8,547.24                                          |  $8,591.68                 |
| R² Score   | 0.66                                                      | 0.66                              |


Both models performed similarly, explaining ~66% of the price variability.
Ridge Regression slightly stabilizes predictions by reducing extreme coefficients.
________________________________________________________________________
4. Key Factors Driving Price
Top predictors of high price (from both models combined):

| Feature                | Influence   |
|------------------------|-------------|
| Ferrari (manufacturer) | Very High   |
| Aston Martin           | High        |
| Tesla                  | High        |
| 12-cylinder engines    | High        |
| Diesel fuel            | Moderate    |
| Datsun                 | Moderate    |
| Morgan	         | Strong      |
| Fiat    	         | Moderate    |

Luxury brands and performance features (i.e. engine type and fuel) command premium prices.
________________________________________________________________________
5. Recommendations for Inventory Strategy
	1.	Focus on Value-Rich Brands: Seek out Ferrari, Tesla, Aston Martin, Porsche for high ROI units—even older models retain high resale value.
	2.	Target Lower-Mileage Inventory: Vehicles with less wear-and-tear (odometer < 100K) fetch consistently higher prices.
	3.	Evaluate Engine and Fuel Type: Diesel, hybrid, and high-cylinder engines trend positively with pricing.
	4.	Track Condition Consistently: Well-documented “excellent” or “good” condition listings show significantly stronger pricing trends.
	5.	Be Selective with Niche Brands: Some brands like Morgan and Fiat trend negatively in resale markets.
________________________________________________________________________
6. Next Steps
	•	Integrate this model into your dealership pricing software or CRM.
	•	Use filters on sourcing platforms to prioritize inventory matching high-value profiles.
	•	Consider expanding this analysis by region or seasonality (future iterations possible).
________________________________________________________________________