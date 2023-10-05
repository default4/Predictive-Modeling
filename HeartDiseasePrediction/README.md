## Overview:

This project focuses on predictive modeling for heart disease using various medical attributes. The primary goal is to develop a machine learning model that accurately predicts the presence of heart disease based on the provided features. The project employs Python programming language and various popular libraries to preprocess the data, train a machine learning model, and evaluate its performance.

## Dependencies:

* Python 3.7+
* Pandas
* Numpy
* Scikit-learn
* Requests

To install the required libraries, run the following command:

$ pip install pandas numpy scikit-learn requests

## Dataset:

The dataset used in this project is the Heart Disease UCI Dataset, which consists of various medical attributes and heart disease status. The dataset can be downloaded directly using the provided URL:

* Heart Disease UCI Dataset: https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/processed.cleveland.data

In this script, the download_data() function downloads the Heart Disease UCI Dataset using the provided URL. The load_data() function reads the data and creates a pandas DataFrame.