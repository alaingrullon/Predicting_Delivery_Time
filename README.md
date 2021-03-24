# Term 2 Data Science Competition
IE HST's Data science competition is a 4 hour end of term kaggle style competition, in which datasets are uploaded from Kaggle and a target variable is to be predicted. 

# Predicting Delivery Time
This years competition involved predicting the delivery time in a town in Pennsylvania, close to New York City. Independent variables about weather, geographical locations, 
van model, number of packages were given with the objective of predciting the delivery time. 

# Methodologies Employed
- Imputation: A simple forward fill given the time series nature of the data and the fact that all missing values were spread out and not together in the time series.
- Dealing with Date Features: Encoded into year, month, day, hour
- Dealing with Categorical: Ordinal encoding for the weather situation feature
- Features Engineering: Created date time features such as Weekend, Workingday, peak_weekend, and peak_workingday. 
- Machine Learning: Train-validation split, xgboost regression for an r2=.68
- Lessons learned: This model did not perform as expected because there was not enough knowledge and time at the moment to implement the Randomized Grid Search with 
                    cross validation, as well as creating daylight features using the astral python package, dealing with cyclical features such as hour, day and month. 
