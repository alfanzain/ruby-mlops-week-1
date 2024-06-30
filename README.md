# MLOps Week 2

## Project

Sentiment Analyst Tweet - Data Preprocessing

## Description

Data Preprocessing, vectorizing, and splitting on tweet for sentiment analyst

## Overview

### Data

This is the sentiment140 dataset. It contains 1,600,000 tweets extracted using the twitter api . The tweets have been annotated (0 = negative, 4 = positive) and they can be used to detect sentiment. https://www.kaggle.com/datasets/kazanova/sentiment140

### Content

It contains the following 6 fields:

1./ target: the polarity of the tweet (0 = negative, 2 = neutral, 4 = positive)

2./ ids: The id of the tweet ( 2087)

3./ date: the date of the tweet (Sat May 16 23:58:44 UTC 2009)

4./ flag: The query (lyx). If there is no query, then this value is NO_QUERY.

5./ user: the user that tweeted (robotickilldozr)

6./ text: the text of the tweet (Lyx is cool)

### What Happened in My Code?

* Getting tweet data from .csv
* Preprocess tweet with `preprocess_tweet`
* First, we convert the tweet to lower text
* Then, regex compile to remove url and mention
* Then, tokenize the tweet into tokens
* Then, stemming and filter out stopwords
* Finally, join the tokens
* On vectorizing process, we use TF-IDF Vectorizer.
