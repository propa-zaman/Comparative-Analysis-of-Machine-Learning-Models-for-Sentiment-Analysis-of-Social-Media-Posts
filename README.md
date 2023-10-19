# Comparative-Analysis-of-Machine-Learning-Models-for-Sentiment-Analysis-of-Social-Media-Posts

This repository contains code and resources for a comprehensive sentiment analysis on three distinct datasets using five different machine learning models.

## Table of Contents
- [Datasets](#datasets)
- [Preprocessing](#preprocessing)
- [Feature Extraction](#feature-extraction)
- [Data Splitting](#data-splitting)
- [Model Fitting and Evaluation](#model-fitting-and-evaluation)

## Datasets

Three datasets were chosen for sentiment analysis:

1. Twitter Sentiments Dataset labeled by Hussein and Sherif
2. Dataset for Sentiment Analysis
3. YouTube Statistics Dataset

From each dataset, we extracted the text/comment column and the corresponding mood column to gain insights into sentiments.

## Preprocessing

Raw text data underwent several preprocessing steps:
1. Removal of stopwords (excluding "not" due to its significance in sentiment context)
2. Replacing non-alphabetic characters with spaces using regular expressions
3. Converting text to lowercase for standardization
4. Tokenization to split the text into individual words
5. Stemming to reduce words to their base/root form

## Feature Extraction

We utilized the Bag-of-Words (BoW) method using scikit-learn's `CountVectorizer` class. Processed text data was converted to a matrix where each row represents a document and columns indicate the word frequency in the document.

## Data Splitting

The datasets were split into training and test sets using scikit-learn's train-test split function. 20% of the data was reserved for testing, ensuring reproducibility by setting a random state of 0.

## Model Fitting and Evaluation

1. **Naive Bayes**: Implemented Gaussian Naive Bayes, a probabilistic classifier leveraging Bayes theorem.
2. **SVM**: Used Support Vector Machine with a linear kernel for classification tasks.
3. **Random Forest**: A classifier was initialized with 100 estimators. Suitable for handling both regression and classification problems.
4. **Gradient Boosting**: A technique capable of handling non-linear associations, large categorical values, missing values, and outliers.
5. **Logistic Regression**: Ideal for binary label datasets, this method is used for regression and predictive analysis.

For each model, we computed a confusion matrix, accuracy score, and classification report for evaluation.

---

To get started, clone this repository and follow the notebook for a step-by-step walkthrough of the project. If you encounter any issues or have suggestions, please raise an issue or submit a pull request.
