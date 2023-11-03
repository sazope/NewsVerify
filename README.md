# Real vs. Fake News Analysis with NLP

This project focuses on analyzing real and fake news articles using Natural Language Processing (NLP) techniques. It involves comparing and gaining insights into the text data from both categories. The project is inspired by the NLTK (Natural Language Toolkit) book and involves the following tasks:


## Introduction

Analyzing and comparing real and fake news has become increasingly important in the age of social media and digital information dissemination. This project uses the ISOT Fake News Dataset, which contains articles from reputable sources like Reuters and articles flagged by fact-checking organizations like Politifact and Wikipedia.

## Data

The dataset consists of about 12,600 articles categorized into real and fake news, saved in two CSV files: "True.csv" and "Fake.csv". Each article includes information such as the title, text, type (real or fake), and publication date. You can find the dataset on Kaggle: [ISOT Fake News Dataset](https://www.kaggle.com/datasets/emineyetm/fakenews-detection-datasets).

## Data Pre-processing

In this project, data pre-processing is crucial to prepare the text data for analysis. The following tasks are performed:

- Data extraction from the "text" field in both CSV files.
- Tokenization, lowercasing, stop word removal, and lemmatization (explained in the Jupyter Notebook).
- Processing options and the reasoning behind them are documented in the Jupyter Notebook.

## Data Analysis

The pre-processed data is analyzed to gain insights into the articles:

- Top 50 stop words by frequency in real and fake news articles.
- Top 50 content words by frequency in real and fake news articles.
- Top 50 bigrams (two-word phrases) by frequency in real and fake news articles.
- Top 50 bigrams by Mutual Information scores (using a minimum frequency of 5) in real and fake news articles.
- Top 50 adjective words in real and fake news articles.
- Additional statistics for each article, such as total words, content words, capitalized words, exclamation marks, and punctuation marks, are saved in CSV files.

## Interpretation of Analysis Results

- **Word Count:** Both real and fake news articles have similar word counts, indicating comparable article lengths.

- **Content Word Count:** The average content word counts are similar, suggesting similar meaningful content in both types.

- **Capitalized Word Count:** Capitalized words are rarely used in both real and fake news articles.

- **Exclamation Mark Count:** Fake news articles use more exclamation marks, indicating a more sensational writing style.

- **Punctuation Count:** Fake news articles use more punctuation marks, suggesting potentially more complex sentences or a sensational writing style.

These findings highlight the linguistic differences between real and fake news articles, offering insights into their writing style and content structure.

