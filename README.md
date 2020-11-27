# Volcanic Eruption Prediction
[link to the competition](https://www.kaggle.com/c/predict-volcanic-eruptions-ingv-oe)

[link to my pre-processed data](https://www.kaggle.com/soheild91/volcan2)

you can also check the first version of my DNN and xgboost method [on kaggel](https://www.kaggle.com/soheild91/ingv-nn-xgb-baseline)

## What I did in this Jupyter Notebook:
- [x] Extracting statistical features from the raw data-set. The raw data-set contains data of 10 different sensors, which are captured with a 1ms interval. I used the mean, median, quantiles, kurtosis ... on the raw data (on moving average with a window length equal to 50) and FTT of it.
- [x] Removing data with variance equal to zero or correlation more than 0.99
- [x] Extracting important features using built-int xgboost method
- [x] Performing hyperparameter tuning by using Optuna
- [x] Using StraightKfol for training to keep similar distribution over the folds
