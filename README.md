# kkbox
This repository shows step-by-step my approach of [kkbox churn prediction challenge](https://www.kaggle.com/c/kkbox-churn-prediction-challenge) on kaggle

## Installation

1. Clone the github repo, go to the folder
2. Download the [data from kaggle](https://www.kaggle.com/c/kkbox-churn-prediction-challenge/data) 
3. Create a `data` folder and `submissions` folder. Move data to data folder.

## Usage
Run each notebook to see step by step

1. kkbox_EDA.ipynb - explores possible trends on preprocesses each data file
2. features.ipynb - merges and cleans the data
3. feature_selection.ipynb - stepwise logistic regression to subset relevant features
4. train/XGBoost.ipynb - trains and creates submission

XGBoost, gradient boosting classifier, neural networks, AdaBoost and logistic regressions were fitted, XGBoost created highest score.

## Credit

Author - Michael Ko
