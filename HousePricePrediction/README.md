## Overview:

This project focuses on predictive modeling and regression analysis for house prices. The primary goal is to develop a machine learning model that accurately predicts house prices based on various features. The project employs Python programming language and various popular libraries to preprocess the data, train a machine learning model, and evaluate its performance.

## Dependencies:

* Python 3.7+
* Pandas
* Numpy
* Scikit-learn
* Requests

To install the required libraries, run the following command:

$ pip install pandas numpy scikit-learn requests

## Dataset:

The dataset used in this project is the Boston Housing Dataset, which consists of various housing features and prices in the Boston area. The dataset is available directly through scikit-learn's built-in dataset loader. More information about the dataset can be found at this URL: https://archive.ics.uci.edu/ml/datasets/Housing

In this script, the load_data() function loads the Boston Housing Dataset using scikit-learn's built-in dataset loader. The main() function splits the data, trains a Linear Regression model, and evaluates the model.