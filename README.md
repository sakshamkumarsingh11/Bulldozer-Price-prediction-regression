# Bulldozer Price Prediction (Regression)

This project is based on the **Bluebook for Bulldozers** dataset.  
The goal is to predict the sale price of bulldozers using historical auction data.

## Dataset
- Source: Kaggle – Bluebook for Bulldozers
- Type: Structured tabular data
- Target variable: `SalePrice`

## What was done
- Loaded and explored the dataset using pandas
- Parsed and extracted features from the `saledate` column (year, month, day, etc.)
- Handled missing values:
  - Numeric features filled using median
  - Missing-value indicator columns added
- Converted categorical features into numeric form using pandas categorical codes
- Split data into training and validation sets
- Trained a `RandomForestRegressor`
- Tuned hyperparameters using `RandomizedSearchCV`
- Evaluated the model using RMSLE
- Generated predictions on the test dataset

## Model
- Algorithm: Random Forest Regressor
- Evaluation metric: RMSLE
- Best achieved score: ~0.141

## Notes
- Preprocessing was done using a custom function (no sklearn Pipeline was used)
- Feature engineering and missing value handling were performed manually
- This project follows the approach taught in the Zero to Mastery Machine Learning course

## Status
- Kaggle competition is closed, so submissions are not accepted
- Model was evaluated locally

