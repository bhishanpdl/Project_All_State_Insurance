<h1 style="background-color:tomato;">Project Description</h1>

- Project date: Apr 3, 2020
- Readme updated: Oct 19, 2020

[The Allstate Corporation](https://www.allstate.com/) is an American insurance company that is in the United States. The company also has personal lines insurance operations in Canada.

Data Source Kaggle: https://www.kaggle.com/c/allstate-claims-severity/data


<h1 style="background-color:tomato;">Approach</h1>

Here, in this linear regression machine learning problem, I tried various approaches to predict the target variable "loss" from given continuous features (`cont`) and categorical features (`cat`).

Rather than building one huge notebook for data processing, hyperparameter tuning, modelling, and model evaluation, I break up the project into EDA, Cleaning and, Modelling parts.

<h1 style="background-color:tomato;">Data Cleaning</h1>

Here, I did following cleaning:
- Box-Cox transform high skewed continuous variables
- One hot encoding categorical variables
- Missing values imputation.

<h1 style="background-color:tomato;">Modelling</h1>

In this project I used following procedure for modelling the problem:
- Choose boxcox transformed continuous features.
- Choose One hot encoded categorical features.
- Standard Scaling the data.
- Log transformation of Target.

Algorithms Used:
- Random Forest Regressor
- Extra Tree Regressor
- Xgboost Regressor
- Stacking of these three estimators

<h1 style="background-color:tomato;">Results</h1>

| Model | 2-Fold Cross Validation MAE | Time Taken|
| :---| ---:| ---: |
| Random Forest | 1292.87  | 1min 37s|
| Extra Trees |1243.44  | 6min 32s|
| Xgboost |1156.78  | 12min 25s|
| Stacking | 1165.00 | 55.5 s|