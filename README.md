# Amazon Book Reviews Sentiment Analysis

## Project Overview

Analyze **1.3M+ Amazon book reviews** using Python, NLTK, and VADER.

## Key Skills

- Python
- Data Analysis
- Natural Language Processing
- Sentiment Analysis



Amazon Book Reviews Sentiment Analysis

A Python NLP project analyzing 1.3M+ Amazon book reviews to identify customer sentiment, frequently used words, and review patterns using NLTK and VADER.

Project Overview

Customer reviews provide valuable insights into product satisfaction and customer preferences. This project analyzes Amazon book reviews to understand reader sentiment and identify recurring themes in highly rated reviews.

The workflow combines data cleaning, text preprocessing, sentiment classification, and data visualization to turn unstructured review text into actionable insights.

Key Highlights
Processed 1.3M+ reviews after removing duplicate and missing records.
Applied text preprocessing using Pandas, regular expressions, and NLTK.
Classified reviews as positive, negative, or neutral using VADER.
Identified frequently occurring words in book reviews.
Created word clouds and sentiment distribution visualizations.
Explored review patterns across book categories.
Business Questions
Which words appear most frequently in book reviews rated above 3 stars?
What is the distribution of positive, negative, and neutral sentiment?
How does sentiment vary across book categories?
Dataset

The project uses an Amazon book reviews dataset from Kaggle, containing review text, ratings, book titles, authors, categories, and related metadata.

Features Used
Feature	Description
Title	Book title
review/score	User-provided book rating
review/text	Written customer review
authors	Book author information
categories	Book category or genre
ratingsCount	Rating-count metadata
Dataset Source

Amazon Book Reviews Dataset on Kaggle

The original dataset is not included in this repository because of its size. Download it from the original source before running the notebook.

Project Structure
amazon-book-reviews-sentiment-analysis/
├── README.md
├── requirements.txt
├── .gitignore
├── notebooks/
│   └── sentiment_analysis.ipynb
├── data/
│   └── README.md
└── images/
    ├── sentiment_distribution.png
    ├── word_cloud.png
    └── frequent_words.png


The images/ directory will contain exported charts. The data/ directory contains dataset instructions rather than the raw CSV files.

Analysis Workflow
1. Data Preparation
Combined review data with book metadata using book titles.
Selected relevant review and book attributes.
Removed duplicate records and rows with missing values.
Retained 1,325,890 reviews after preprocessing.
2. Text Preprocessing
Converted review text to lowercase.
Removed URLs, punctuation, special characters, and numeric terms.
Removed English stopwords using NLTK.
Generated cleaned text for sentiment analysis and word-frequency exploration.
3. Sentiment Analysis

Applied VADER, a lexicon-based sentiment analysis tool, to calculate a compound sentiment score for each cleaned review.

Sentiment	Compound Score
Positive	≥ 0.05
Neutral	> −0.05 and < 0.05
Negative	≤ −0.05
4. Exploratory Text Analysis
Calculated frequent words in review text.
Generated a word cloud for reviews rated above 3 stars.
