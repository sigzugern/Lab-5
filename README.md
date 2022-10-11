# Lab 5 - Predicting Galaxies/Stars/Quasars with XGBoost

In this lab, we will use XGBoost to predict whether a galaxy is a star, a galaxy, or a quasar. We will use a subset of the [SDSS DR14](https://www.sdss.org/dr14/) dataset, which contains 10000 entries of galaxies, stars, and quasars. The dataset is available on [Kaggle](https://www.kaggle.com/lucidlenn/sloan-digital-sky-survey).

This type of machine learning problem is called a **multi-class classification** problem and is **supervised machine learning**. We will use the XGBoost library to train a model to predict the class of a galaxy based on its features.


We will be introducing the following concepts:
    * F1 score
    * Cross-validation
    * Confusion matrix
    * Feature importance
    * Hyperparameter optimization with Optuna

## F1 Score

F1 score is a metric that is used to evaluate the performance of a model. It is a weighted average of the precision and recall. This is useful when we have an uneven class distribution. In this lab, we will use F1 score to evaluate the performance of our model. The F1 score is the go-to metric for multi-class classification problems.

## Cross-validation

Cross-validation is a technique used to evaluate the performance of a model. It is used to estimate the performance of a model on unseen data. We will use cross-validation to evaluate the performance of our model. Cross-validation uses the entire dataset to train and evaluate the model. This is different from train-test split, which uses a subset of the dataset to train and evaluate the model.

## Confusion matrix

A confusion matrix is a table that is used to describe the performance of a classification model. Each row of the matrix represents the instances in a predicted class while each column represents the instances in an actual class. The confusion matrix tells us how many instances were correctly classified and how many were misclassified, and exactly how they were misclassified.

## Feature importance

Feature importance is a metric that is used to evaluate the importance of each feature in a model. It is used to determine which features are most important in making predictions. If a model is not performing well, we can use feature importance to determine which features are not contributing to the model's performance.

## Optuna

Optuna is a hyperparameter optimization library that is designed to be easy to use and efficient. It is a good alternative to GridSearchCV and RandomizedSearchCV as it is more efficient and can be used to optimize more complex hyperparameters, this is because it uses Bayesian optimization.
