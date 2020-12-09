## Introduction:

In machine learning, there are many algorithms to choose from. What algorithm to choose can be filtered analysing the problem and the data. Oftentimes, after the filtration process, we are still left with multiple algorithms to select from. Therefore, whenever feasible, training data on different algorithms and tuning each parameter of the algorithm is necessary. In this report, we dive into the practice of using and tuning different models. The report will go through each step involved in solving machine learning problem. First, we will define a problem. Second, we will tweak our data to better fit our problem. Third, we will define and tun the models. Lastly, we will compare and evaluate models.
The 3 models to be used in the report are:
1.	XGBoost
2.	Logistic Regression
3.	Neural network

## Problem Formulation:

The problem presented in the report is Jane Street Market Prediction  competition from Kaggle. We will tweak and simplify the problem. The competition involves in predicting whether a trade will be profitable or not given the input. The evaluation in the competition is using a utility function but for this experiment, we will tweak our evaluation.
Data used to train/validation/test the model is stored in the file name train.csv. The data contains date, weight, multiple resp (return) columns, and multiple feature columns. Each row represents a trade and different resp values represent the different returns. For simplicity, we will ignore the multiple resp value and weights. We will use one of the resp column to evaluate if the trade should be taken or not. If the resp is below 0, we will label 0, and 1 if resp above 1. The goal of our model will be to predict if a given trade should be 0 or 1. In other words, this will be a binary classification problem.
In the end we will compare which model makes more money or in other words which one can predict profitable trade more while minimizing losing trades.  Whichever model does it the best will be classified as a better model.

## Approaches:

For a full detailed report on the experiment, please check the report.pdf or the jupyter notebook.

Thank you for reading!
