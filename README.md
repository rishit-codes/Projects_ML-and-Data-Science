# Teen Phone Addiction Analysis
This project explores the impact of smartphone usage on teenagers' lifestyle and mental health using the Teen Phone Addiction dataset. It applies machine learning models like Linear Regression, Ridge, Lasso, and ElasticNet to predict addiction levels and understand influencing factors.

## Exploratory Data Analysis
- Distribution plots for all numeric columns
- Correlation heatmap
- Pair plots for selected features
- Box plots to compare usage patterns vs addiction levels

## Models Used
- Linear Regression (Baseline)
- Ridge Regression (with cross-validation)
- Lasso Regression (with alpha tuning)
- ElasticNet (best performance with R² ≈ 0.74)

All models were evaluated using:
- R² Score
- Mean Absolute Error

ElasticNet performed the best after hyperparameter tuning.


## Acknowledgements

- Kaggle for the dataset
- Scikit-learn for ML models
- Seaborn & Matplotlib for visualizations
