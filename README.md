# Capstone 2: NLP - Classify Fake News

### Determine if an article is fake news or not.

## Purpose
The aim of this project was to identify whether a given news article is real news or fake news.

## Data
Data was downloaded from [Kaggle](https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset) 
Data contains a total of 44898 news articles. Target classes as well balanced with 23481 articles classified as fake and 21417 classified as real.For our analysis the fake news table and real news tables were merged to form a single table.

## Feature Engineering
Implemented the following ideas to obtain relevant features from the dataset:
-Text/NLP based features:
  1. Count of words
  1. Count of words starting with upper case 
  1. Count of characters
  1. Average length of the words
  1. Punctuation count
  1. Frequency distribution of Part of Speech Tags:
    1. Noun Count
    1. Verb Count
    1. Adjective Count
    1. Adverb Count
    1. Pronoun Count
-TF-IDF features as vectors


## Date processing
The following text 

## Model used
Initially decided to go with Logistic Regression, but the model did not perform well. Achieved better results with CatBoost Classifier implemented using PyCaret library.

## Result
Accuracy is not a good performance measure due to the imbalanced nature of the data hence used AUC score. 
Tuned CatBoost classifier achieved:
### AUC: 0.724
