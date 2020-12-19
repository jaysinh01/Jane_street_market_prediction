## Introduction:

In machine learning, there are many algorithms to select for a model. What algorithm to choose can be filtered by analysing the problem and the data. After the filtration process, we are often left with multiple algorithms to select for a model. In this case, if feasible, we should train and tune multiple algorithms to find the best algorithm. In this report, we dive into the practice of using and tuning different models. The report will go through each step involved in solving a machine learning problem:
  1.  We will define a problem.
  2.	We will tweak our data to fit the problem.
  3.	We will define and tune the models.
  4.	We will compare and evaluate the models.
  
The three models to be used in the report are:

  1.	XGBoost
  2.	Logistic Regression
  3.	Neural network


## Problem Formulation:

The problem presented in the report is from Jane Street Market Prediction competition. The competition involves in predicting whether a trade will be profitable or not given the input. The evaluation in the competition is using a utility function however our evaluation will simply be which model has a greater profit potential.
Data used to train/validation/test the model contains date, weight, 4 resp (return) columns, and 130 feature columns. Each row represents a trade and different resp values represent the different returns. For simplicity, we will ignore the multiple resp value and weights. We will use one of the resp column to evaluate if the trade should be taken or not. If the resp is below 0, we will label 0, and 1 if resp above 1. The goal of our model will be to predict if a given trade should be 0 or 1. In other words, this is a binary classification problem.
In the end, we will compare which model can predict profitable trade more while minimizing losing trades.  Whichever model does it the best will be classified as a better model.

## Approaches:

For a full detailed report on the experiment, please check the report.pdf or the jupyter notebook.

Thank you for reading!
