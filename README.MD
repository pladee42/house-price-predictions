---

# House Price Prediction

This project is a Kaggle competition entry for predicting house prices based on a variety of features. The objective is to build and evaluate machine learning models to achieve the most accurate predictions for house prices.

## Project Overview

The project leverages several machine learning and deep learning models to predict house prices. Key highlights include:

- **Data Preprocessing**: Cleaning and preparing data to handle missing values, outliers, and feature engineering.
- **Model Training**: Implementation of multiple regression and deep learning models.
- **Evaluation**: Models are evaluated using metrics like R-squared, Mean Squared Error (MSE), Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE).
- **Submission**: Predictions are saved in a CSV format for Kaggle submission.

## Models Used

The following models were implemented and tuned:

1. **Linear Regression**
2. **Random Forest Regressor**
3. **XGBoost Regressor** (Best-performing model)
4. **Deep Learning** using Keras with hyperparameter tuning.

## Evaluation Metrics

- **R-squared (R²)**: Measures the proportion of variance explained by the model.
- **MSE**: Mean Squared Error to assess the average squared error.
- **MAE**: Mean Absolute Error to measure the average magnitude of errors.
- **RMSE**: Root Mean Squared Error as a measure of accuracy.

### Results

| Model               | R²      | MSE   | MAE   | RMSE  |
|---------------------|---------|-------|-------|-------|
| Linear Regression   | 0.7711  | 0.0404| 0.1009| 0.2010|
| Random Forest       | 0.8430  | 0.0277| 0.1069| 0.1665|
| Deep Learning       | 0.6751  | 0.0574| 0.1746| 0.2395|
| **XGBoost**         | **0.8584**| **0.0250**| **0.1006**| **0.1581**|

## Usage Instructions

### Dependencies

The project uses Python and requires the following libraries:
- `numpy`
- `pandas`
- `scikit-learn`
- `xgboost`
- `keras`
- `matplotlib`

Install the dependencies with:
```bash
pip install numpy pandas scikit-learn xgboost keras matplotlib
```

### Running the Project

1. **Data Preparation**: Place the dataset in the appropriate directory and preprocess it in the notebook.
2. **Model Training**: Run the notebook cells to train the models.
3. **Hyperparameter Tuning**: Leverage `GridSearchCV` for optimizing model parameters.
4. **Prediction Submission**: Generate predictions using the best model (XGBoost) and save them to `submission.csv`.

### Output

The best model, XGBoost, produces predictions with an R-squared score of 0.8584 on the validation set. The predictions are exported as a CSV file ready for Kaggle submission.

---