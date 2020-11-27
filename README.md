# Volcanic Eruption Prediction
[link to the competition](https://www.kaggle.com/c/predict-volcanic-eruptions-ingv-oe)

[link to my pre-processed data](https://www.kaggle.com/soheild91/volcan2)

## What I did in this Jupyter Notebook:
- [x] extracting statestical features from the raw data-set. the raw data-set, containes data of 10 different sensors which are captured with a 1ms interval. I used mean, median, quantiles, kurtosis ... on the raw data (on moving average with a window lenght equal to 50) and FTT of it.
- [x] removing data with variance equal to zero or correlation more than 0.99
- [x] extracting important features using built-int xgboost method
- [x] performing hyper-parameter tuning by using Optuna
- [x] using StraightKfol for training to keep similar distribution over the folds
