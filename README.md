# IMDB Movie Review Sentiment Analysis

## Overview

This project performs sentiment analysis on movie reviews from the IMDB dataset using Natural Language Processing (NLP) and Machine Learning techniques.

The objective is to classify movie reviews as either positive or negative based on the textual content of the review.

The project compares multiple text representation and machine learning pipelines to identify an effective approach for sentiment classification.

## Objective

The main objectives of this project are to:

- Process and clean unstructured text data.
- Apply Natural Language Processing techniques to movie reviews.
- Convert text into numerical features using text vectorization techniques.
- Train multiple machine learning classification models.
- Compare model performance using standard evaluation metrics.
- Identify the best-performing sentiment classification approach.

## Dataset

The dataset contains **50,000 IMDB movie reviews**.

Each review contains:

- `review` – The text of the movie review.
- `sentiment` – The sentiment label of the review.

### Sentiment Labels

| Sentiment | Label |
|---|---|
| Positive | 1 |
| Negative | 0 |

## Technologies Used

- Python
- Pandas
- NumPy
- NLTK
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## NLP Preprocessing

The text data was processed using the following steps:

1. Converted text to lowercase.
2. Removed unnecessary characters and noise.
3. Tokenized the reviews.
4. Removed stop words.
5. Applied lemmatization.
6. Created cleaned review text for further analysis.

## Feature Extraction

The project uses text vectorization techniques to convert reviews into numerical features:

### Bag of Words

Represents text based on the frequency of words appearing in each review.

### TF-IDF

Assigns importance to words based on their frequency within a review and across the entire dataset.

## Machine Learning Models

Multiple classification pipelines were developed and compared using:

- Multinomial Naive Bayes
- Logistic Regression

The models were evaluated using different text representation techniques, including:

- Bag of Words
- TF-IDF

This resulted in a comparison of four sentiment classification pipelines.

## Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

## Project Workflow

```text
IMDB Reviews
      ↓
Data Cleaning
      ↓
Text Preprocessing
      ↓
Tokenization and Lemmatization
      ↓
Feature Extraction
(Bag of Words / TF-IDF)
      ↓
Machine Learning Classification
      ↓
Model Evaluation
      ↓
Sentiment Prediction
