# brazilian_cities_IDHM

A descriptive analysis and machine learning application to predict the IDHM of brazilian cities based on the following dataset from kaggle:

https://www.kaggle.com/crisparada/brazilian-cities

This dataset has numerical and categorical real world data with all kind of funny stuff to be dealt with. This project reaally helped me learn how to build pipelines using only sklearn estimators and transformers. I believe it's a good example of what can be done structuring pipelines with sklearn's Pipeline() and ColumnTransformer().

The model consists of a VotingRegressor with 4 estimators:
  - RandomForest
  - GrandientBoosting
  - XGBoost
  - LightGBM

The last one tuned with bayesian optimization (Optuna) and the whole thing got a r2 score of 0.9+.

I'm going to optuna the hell out of the other 3 soon, excited to see how far can it go. Kind of regreting to spent so much time and effort in a dataset that doesn't have a kaggle competition jajajajajaja just kidding, it was really fun to play with! 
