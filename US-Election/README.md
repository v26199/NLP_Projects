# Optimizing Political Campaigns with Twitter Sentiment Analysis

## Introduction
This project demonstrates how to perform sentiment analysis on tweets related to the 2020 US presidential elections using Natural Language Processing (NLP) techniques. The aim is to derive actionable insights that can help optimize political campaigns. 

## Data Source
The dataset used in this project is a collection of tweets gathered over three weeks around the 2020 US presidential elections. It can be downloaded from [Kaggle](https://www.kaggle.com/datasets/manchunhui/us-election-2020-tweets/data).

## Table of Contents
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Text Pre-processing](#text-pre-processing)
- [Intro to Sentiment Analysis](#intro-to-sentiment-analysis)
- [Sentiment Analysis with TextBlob](#sentiment-analysis-with-textblob)
- [Sentiment Analysis with VADER](#sentiment-analysis-with-vader)
- [Sentiment Analysis with Flair](#sentiment-analysis-with-flair)
- [Comparing Sentiment Analysis Libraries](#comparing-sentiment-analysis-libraries)
- [Actionable Insights from Sentiment Analysis of Tweets](#actionable-insights-from-sentiment-analysis-of-tweets)
- [Setup](#setup)


## Exploratory Data Analysis
First, we conduct exploratory data analysis (EDA) to understand basic metrics such as the number of tweets and the date range covered by the dataset.

## Text Pre-processing
Text pre-processing is essential for cleaning the data. This involves:
- Removing stop words
- Converting words to their base forms (e.g., plurals to singular)
- Removing URLs, mentions, and special characters

## Intro to Sentiment Analysis
Sentiment analysis involves determining the emotional tone behind a body of text. It is commonly used to understand the sentiment expressed in tweets, which can be positive, negative, or neutral.

## Sentiment Analysis with TextBlob
[TextBlob](https://textblob.readthedocs.io/en/dev/) is a simple library for processing textual data. It provides a consistent API for diving into common NLP tasks.

## Sentiment Analysis with VADER
[VADER (Valence Aware Dictionary and sEntiment Reasoner)](https://github.com/cjhutto/vaderSentiment) is a lexicon and rule-based sentiment analysis tool that is specifically attuned to sentiments expressed in social media.

## Sentiment Analysis with Flair
[Flair](https://github.com/flairNLP/flair) is a powerful NLP library. It provides a simple interface for state-of-the-art models, allowing us to perform sentiment analysis with high accuracy.

## Comparing Sentiment Analysis Libraries
We compare the results from TextBlob, VADER, and Flair to determine which library best suits our dataset. This involves analyzing the sentiment distribution and accuracy of each library.

## Actionable Insights from Sentiment Analysis of Tweets
Given the context of a political campaign, we derive actionable insights from the sentiment analysis results. The goal is to find strategies to increase our candidate's voter base.

## Setup
To set up the environment and run the analysis, follow these steps:

1. **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```

2. **Download NLTK data**
    ```python
    import nltk
    nltk.download('vader_lexicon')
    nltk.download('stopwords')
    nltk.download('punkt')
    nltk.download('averaged_perceptron_tagger')
    nltk.download('wordnet')
    ```

4. **Load Dataset**
    Download the dataset from [Kaggle](https://www.kaggle.com/datasets/manchunhui/us-election-2020-tweets/data) and place it in the project directory.

5. **Run the Analysis**
    Execute the provided Jupyter notebooks or Python scripts to perform EDA, text pre-processing, sentiment analysis, and visualization.

## License
This project is licensed under the MIT License.
