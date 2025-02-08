# ML_regression_tomatometer_rating_zoho_assessment
-Dataset link-->[https://docs.google.com/spreadsheets/d/1l6DSMNy6vVkaVqk2eqEo1n2BAyeEPbtB/edit?usp=sharing&ouid=102777560562290734716&rtpof=true&sd=true]
## Project Overview
### Project demo -[]
### Project Objective
- To Predict the **'audience_rating'** dependant variable from the given RottenTomatoes movies dataset - Regression Problem
- To build a machine learning model using **SCIKIT-LEARN(train and test splits), Pytorch(train and test splits) and Tensorflow(train,validation and test splits).**

- ## Classification ROCAUC score and Accuracy Table for oversampled dataset
|    Model             |  Train(R2-score)			|  Train(RMSE)   |Test(R2-score) |Test(RMSE)   
| :------------------- | -----------------  |-----------------|-----------------|-----------------:  
| PolynomialRegression(degree=2)|	0.6198	  |      12.583         |0.5304            |13.95|    
|Linear Regression	        |0.5786	             |13.2469	| 0.5041	|      14.3346     |
| LassoRegression	|      0.5779	       |13.257	               |0.5104	      |14.2436| 
|RidgeRegression	  |  0.5786	     |  13.2476	   |    0.5041	|         14.3346|
|ElasticNetRegression             |     	0.5786	        |13.2476	          |0.5065	     |14.3002             |
| RandomForestRegressor	    |0.603	               |12.853	  |0.5344	                            |13.89| 
| HistGradientBoostingRegressor	   |0.8457	              |8.0151	  |0.5577	                             |13.537| 
| XGBRegressor	    |0.1040               |	19.316				  |0.0960	                           |19.3538| 
| **Linear Regression (BEST FEATURES)**		    |0.5645	           |	13.466	  			  |0.4930	                            |14.4933| 

## Results
- This dataset is a **Human behaviour** dataset, I tried to get the best model performance by using various techniques, but was able to get an R2 score ~0.50(both train and test sets).Kindly ref this link:[https://statisticsbyjim.com/regression/how-high-r-squared/]
- LinearRegression,LassoRegression ,PolynomialRegression and RandomForestRegressor models have given the best R2 scores which approximates 0.57 in the train sets and 0.50 in the test sets respectively.
- The Ensemble algorithms likeHistGradientBoostingRegressor scores is also noteworthy, R2 scores which approximates 0.90 in the train sets and 0.56 in the test sets respectively.
- The RMSE score is ~14, which implies that the difference in most of the predicted and actual values lies between the range +/-14.
- The XGBRegressor has not been able to find the pattern and has performed poorly.
- The best_features are:'tomatometer_rating','genre','directors','studio_name', 'runtime_in_minutes','in_theaters_year','tomatometer_status','tomatometer_count'
## Hope the results are good!!!
