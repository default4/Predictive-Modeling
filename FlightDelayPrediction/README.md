## Overview:

The project aims to predict house prices using machine learning algorithms. Various features such as the number of bedrooms, square footage, and location are used to make predictions. The Python programming language and several popular libraries are employed to preprocess the data, train a machine learning model, and evaluate its performance.

## Dependencies:

* Python 3.7+
* Pandas
* Numpy
* Scikit-learn
* Requests

To install the required libraries, run the following command:

$ pip install pandas numpy scikit-learn requests

## Dataset:

The dataset used in this project is the California Housing dataset, which contains information on housing prices in California. The dataset can be downloaded directly using the provided URL:

* California Housing Dataset: https://raw.githubusercontent.com/ageron/handson-ml2/master/datasets/housing/housing.csv

In this script, the download_data() function downloads the California Housing dataset using the provided URL. The load_data() function reads the data and creates a pandas DataFrame. The script includes preprocessing steps, a RandomForestRegressor model, and evaluation metrics.

