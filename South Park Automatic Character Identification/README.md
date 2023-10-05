# Automatic Character Identification from TV Show Lines

## Overview

The "Automatic Character Identification from TV Show Lines" project aims to leverage Natural Language Processing (NLP) techniques to predict which character from a TV show might have spoken a given line. This intricate task of text classification involves numerous steps, from data preprocessing to model optimization.

## Dataset Description

Our dataset provides a rich collection of lines from various characters spanning different episodes and seasons of a TV show. Each record in the dataset carries crucial information about the season, episode number, the character's name, and the line they articulated.

## Detailed Project Workflow

### Data Preprocessing

In the initial phase of our project, we concentrated on refining our dataset. We began by eliminating any records with missing data to ensure consistency. To further sanitize our text data, we converted all the lines to lowercase, ensuring a uniform representation. Following this, we stripped the text of any special characters, numbers, and punctuations. The purpose behind this meticulous cleaning was to focus solely on the words spoken, disregarding any extraneous elements. Finally, we tokenized the text, breaking down each line into its constituent words. This granular breakdown facilitated a more profound analysis of the text's structure.

### Feature Extraction

Once our data was preprocessed, the next step was to extract meaningful features that could be fed into our machine learning models. For this, we employed the Term Frequency-Inverse Document Frequency (TF-IDF) method. This technique transformed our tokenized text into vectors, capturing the essence of each word in the context of the entire dataset. The TF-IDF method effectively gauges both the local importance of words (how often a term appears in a particular line) and their global significance (how frequent a term is across all lines).

### Model Selection and Training

With our features ready, we ventured into the model selection phase. We kickstarted our experiments with the Multinomial Naive Bayes classifier, given its renowned efficacy in text classification tasks. However, to optimize our model's performance and computational efficiency, we made a strategic decision to focus our predictions on the top 10 most frequently speaking characters from the show.

Expanding our horizons, we also experimented with the Random Forest and Linear Support Vector Machine (SVM) classifiers. Our evaluations revealed that the SVM, particularly the linear variant, demonstrated superior performance in predicting the characters accurately.

### Hyperparameter Tuning

Recognizing the potential of the SVM model, we dove deeper to fine-tune its performance. Utilizing the GridSearchCV method, we embarked on a journey to discover the optimal hyperparameters for our SVM model. This exhaustive search crowned the hyperparameters \( C = 0.1 \) and `loss = 'squared_hinge'` as the best performers, driving our model's accuracy even higher.

## Results and Insights

Our journey through various models yielded the following accuracies:

- The Multinomial Naive Bayes model, focusing on the top 10 characters, achieved an accuracy of 38.84%.
- The Linear SVM model showcased an impressive performance with an accuracy of 40.71%.
- However, the crown jewel was our Optimized Linear SVM model, which, with the best hyperparameters, reached an accuracy peak of 41.60%.

## Visualizations

To provide a vivid picture of our dataset and model performances, we crafted two primary visualizations:

1. **Character Frequency**: This visualization paints a clear picture of the number of lines spoken by the top 10 characters. It not only offers insights into the dataset's distribution but also sheds light on the characters' prominence in the show.
2. **Model Performance Comparison**: Through this visualization, we juxtaposed the accuracies of our three main models: Multinomial Naive Bayes, SVM, and Optimized SVM. This comparative view aids in understanding the relative strengths of each model and the enhancements brought about by optimizations.
