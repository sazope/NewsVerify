# Real vs. Fake News Analysis and Sentiment-Based Classification

## Introduction

This project combines two distinct yet related tasks: real vs. fake news analysis and sentiment-based text classification. In the era of digital information, it's essential to distinguish between trustworthy news sources and identify the sentiment within text data. We begin with an analysis of real and fake news articles using Natural Language Processing (NLP) techniques and then leverage a sentiment classifier trained on a Twitter Airline Sentiment dataset to detect fake news.

## Real vs. Fake News Analysis

### Data
We start by analyzing the ISOT Fake News Dataset, containing over 12,600 articles categorized as real and fake news, saved in two CSV files: "True.csv" and "Fake.csv." These articles are sourced from reputable outlets like Reuters, as well as articles flagged by fact-checking organizations.

### Data Pre-processing
Data pre-processing is a crucial step to prepare text data for analysis, including data extraction, tokenization, lowercasing, stop word removal, and lemmatization.

### Data Analysis
We perform extensive analysis on the pre-processed data, including:
- Identifying the top 50 stop words and content words by frequency in real and fake news articles.
- Discovering the top 50 bigrams (two-word phrases) by frequency.
- Calculating top 50 bigrams by Mutual Information scores.
- Analyzing the usage of adjective words.
- Collecting additional statistics for each article, such as total words, content words, capitalized words, exclamation marks, and punctuation marks.

### Interpretation of Analysis Results
We highlight key findings that differentiate real and fake news articles, shedding light on linguistic differences, writing styles, and content structures.

## Sentiment-Based Classification

### Data Preprocessing
We then shift our focus to sentiment analysis and classification, starting with the Twitter Airline Sentiment dataset. Data is preprocessed by converting text to lowercase and removing stop words, followed by splitting the data into training and testing sets.

### Experiments
We conduct a series of experiments to develop a sentiment classifier:
1. Experiment with unigram features using CountVectorizer and a Multinomial Naive Bayes classifier.
2. Incorporate bigram features by adjusting ngram_range.
3. Introduce negation handling to improve model understanding.
4. Create a sentiment lexicon using the VADER SentimentIntensityAnalyzer, and train a Logistic Regression model.

### Final Model
We conclude by training a final Multinomial Naive Bayes model using unigram features on the Twitter Airline Sentiment dataset.

## Detecting Fake vs. Real News
With the trained sentiment classifier in place, we apply it to the task of detecting fake vs. real news. We preprocess and tokenize news articles into sentences, using the classifier to determine the sentiment of each sentence. We calculate the average number of positive and negative sentences for both fake and real news articles.

## Conclusion
This project showcases the comprehensive process of analyzing real vs. fake news and building a sentiment-based classification model. Feature selection significantly impacts model performance, and the sentiment lexicon model outperformed other experiments. These models have practical applications in real-world scenarios, such as distinguishing between fake and real news based on sentiment analysis.

With a strong foundation in NLP and sentiment analysis, this project provides valuable insights into the world of digital information and text classification.
