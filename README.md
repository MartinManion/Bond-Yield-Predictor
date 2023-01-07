# Bond-Yield-Predictor
A group project, completed with a partner, for a class in the spring of 2022.
Objective: design a model to predict the yield on bonds using both ESG and traditional data.
Data Source: ESG and financial data were pulled from Bloomberg. Ratings data was pulled from Fitch, S&P, and Moody's.
Data Cleaning: dropped outliers in Yield to Maturity, filled missing Ratings data with 'Missing', dropped sparse columns such as recordID and IssuerName.  
Baseline RSME of 7.38 based on the mean bond yield.
Ran a number of models, including many SKLearn models and Neural Nets using Keras. Also ran models with all data, just ESG data, and just traditional financial data.
Best traditional model: Lasso Regression with Polynomial Features, all data, had an RMSE of 4.26.
Best neural net: neural net with no ESG data had an RMSE of 4.20 (for reference, NN with only ESG data had an RMSE of 6.34).
