# Traffic Speed Prediction (XGBoost and LightGBM)
## Description
The dataset provides the average traffic speed per hour for a major road in Hong Kong from 2017 to 2018. Part of the dataset is provided as the training data, and your task is to predict the rest. 80% of the dataset is provided as the training data and 20% as the testing data, including the timestamp and the corresponding average speed. We sampled the testing data only from the year 2018 to provide you a training dataset that has the complete data spanning the year 2017. However, the speed information is sometimes missing due to device malfunction.
Evaluation Metric: the mean-squared error
## Programming Languages and Required Packages
* Development Environment: Anaconda-Jupyter-notebook
* Programming Language: Python3.7
* Required Packages: math, numpy, pandas, sklearn, scipy, datetime, xgboost, lightgbm

## Prediction Model 
In this project, I used XGBoost regression model and LightGBM regression model to do prediction about the traffic speed. In my implemenetation, there are four main parts. The first one is doing the data preprocessing with training set and test set. The second one is about feature engineering which helps us find the potential relationship between the traffic speed and other factors. For example, the timestamp is whether weeekend or work day, or is whether working hours or non-working hours. The third one is training Models which contains XGboost (Directly Use RandomizedSearch), XGboost (Step by Step to Use GridSearch) and LightGBM (Step by Step to Use GridSearch). The last one is doing the prediction by using the best parameters found by the above tuning methods and saving the result into test.csv.  

## Notes
#### Reference
* XGBoost vs LightGBM: https://blog.csdn.net/weixin_41089007/article/details/97046470
* XGBoost Model Tuning Parameters: https://blog.csdn.net/sinat_35512245/article/details/79700029
* LightGBM Model Tuning Parameters: https://www.cnblogs.com/bjwu/p/9307344.html


## Result:
1. how to run it to reproduce my result:
```
Traffic_Speed_Prediction_based_on_XGBoost_and_LightGBM.ipynb
├── Initiate Training Set and Test Set: Basic Data Preprocessing
├── Feature Engineering
├── Dividing Training Dataset
├── XGboost--Directly Use RandomizedSearch
├── XGboost--Directly Use RandomizedSearch--Prediction and Output
├── XGboost--Step by Step to Use GridSearch
├── XGboost--Step by Step to Use GridSearch--Prediction and Output
├── LightGBM--Step by Step to Use GridSearch
└── LightGBM--Step by Step to Use GridSearch--Prediction and Output
```

2. The resulting test.csv file. This should be identical to your final submission.

