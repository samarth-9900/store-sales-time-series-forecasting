# Store Sales Time Series Forecasting

A time series forecasting project for predicting store-level sales using the Kaggle Store Sales dataset.

## Approach

- Processed and interpolated missing oil-price data
- Merged oil prices with the sales data using date
- Created a chronological train-validation split
- Engineered calendar and time-based features
- Used store number and product family as categorical features
- Trained a CatBoost Regressor
- Evaluated performance using RMSLE
- Generated predictions for the Kaggle test set
- Created the final Kaggle submission file

## Features

- Store number
- Product family
- On-promotion count
- Oil price
- Year
- Month
- Day
- Day of week
- Days since start

## Model

**CatBoost Regressor**

- Iterations: 200
- Learning rate: 0.05
- Depth: 10
- Loss: RMSE

## Validation

A chronological validation set covering **August 1–15, 2017** was used.

**Validation RMSLE: 0.9863**

## Dataset

Kaggle: Store Sales - Time Series Forecasting

## Files

```text
store-sales-time-series-forecasting/
│
├── model-01.ipynb
└── README.md
