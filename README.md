# kkbox
This repository shows step-by-step my approach of [kkbox churn prediction challenge](https://www.kaggle.com/c/kkbox-churn-prediction-challenge) on kaggle

## Installation

1. Clone the github repo, go to the folder
2. Download the [data from kaggle](https://www.kaggle.com/c/kkbox-churn-prediction-challenge/data) 
3. Create a `data` folder and `submissions` folder. Move data to data folder.

## Notes

All datasets provided by kaggle in this competition is way too big to post. Thus, in order to replicate my take on the challenge, the files must be downloaded from kaggle. Additionally, there is one file called userlog which is way too big for my computer to process. The datafile is over 300 million rows and 6.65 GB. Thus I forked another kaggler's [output](https://www.kaggle.com/kevinbonnes/r-incorporating-user-logs-csv-in-your-model ) of userlog (mean of num_unq and total_secs). This dataset should also be stored in data.

`Models` and `Submissions` store prediction of train dataset and test dataset. These were made in case someone decided to use them in ensemble stacking. I do not think that ensemble stacking wil help, since I believe that the train dataset is somewhat different from the test (which is why the logloss of test is significantly larger than train despite cross-validation).

## Usage
Run each notebook to see step by step

1. kkbox_features_EDA - summarizes all datafiles, basic feature engineering, and some data visualization
2. feature_selection.ipynb - stepwise logistic regression to subset relevant features
3. train/XGBoost.ipynb - trains and creates submission

XGBoost, gradient boosting classifier, neural networks, AdaBoost and logistic regressions were fitted, XGBoost created highest score.

## Results

Last checked public leaderboard score was top ~30%. Private leaderboard and public leaderboard can differ quite a bit, so this is not the final standing.

## Credit

Author - Michael Ko

Any suggestions, comments and thoughts are welcomed! Contact me mlko53 [at] stanford [dot] edu
