# Heart Disease Risk Prediction

A logistic regression model that identifies the strongest behavioral and health predictors of heart disease using CDC BRFSS 2015 survey data (253,680 respondents).

## Methods
- 70/30 train/test split
- Baseline logistic regression on all 21 features
- Forward stepwise feature selection (5-fold CV, ROC AUC scoring)
- Final model: top 14 features, standardized

## Results
- Test ROC AUC: **~0.845**
- Top predictors: general health status, stroke history, high blood pressure, high cholesterol, age

## Key Insight
Heavy alcohol consumption showed a *negative* correlation with heart disease, likely due to survivorship bias and the younger average age of heavy drinkers in the sample, not a protective effect.

## Limitations
- Self-reported, cross-sectional data — associations, not causation
- Logistic regression prioritized here for interpretability over raw predictive power

## Data
[CDC BRFSS 2015](https://www.cdc.gov/brfss/annual_data/annual_2015.html) (via Kaggle)

## Author
Nancy Le