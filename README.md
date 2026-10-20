## Amazon Book Reviews Sentiment Analysis

A Python NLP project analyzing 1.3M+ Amazon book reviews to identify customer sentiment, frequently used words, and review patterns using NLTK and VADER.

Overview

Customer reviews provide useful insights into product satisfaction and customer preferences. This project analyzes Amazon book reviews to understand the sentiment expressed by readers and identify recurring themes in highly rated reviews.

The workflow combines data cleaning, text preprocessing, lexicon-based sentiment classification, and visualization to turn unstructured review text into interpretable insights.

Project Highlights
Processed 1.3M+ reviews after removing duplicate and missing records.
Applied text preprocessing using Pandas, regular expressions, and NLTK.
Classified reviews as positive, negative, or neutral using VADER compound scores.
Identified frequently occurring words in review text.
Generated word clouds and sentiment distribution visualizations.
Explored review patterns across book categories.
Business Questions
Which words appear most frequently in reviews rated above 3 stars?
What is the distribution of positive, negative, and neutral sentiment?
How does sentiment vary across book categories?
Dataset

The project uses an Amazon book reviews dataset from Kaggle, containing review text, ratings, book titles, authors, categories, and related metadata.

Features used:

Title — book title
review/score — user-provided rating
review/text — written review
authors — book author information
categories — book category or genre
ratingsCount — book rating-count metadata

Source: Amazon Book Reviews Dataset on Kaggle

The original dataset is not included in this repository because of its size. Download it from the source before running the notebook.

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


The images/ files are optional until you export your charts. The data/ folder contains dataset instructions, not the raw CSV files.

Analysis Workflow
1. Data Preparation
Combined book reviews with book metadata using the book title.
Selected relevant review and book attributes.
Removed duplicate records and rows with missing values.
Retained 1,325,890 records after preprocessing.
2. Text Preprocessing
Converted review text to lowercase.
Removed URLs, punctuation, special characters, and numeric terms.
Removed English stopwords using NLTK.
Generated cleaned review text for further analysis.
3. Sentiment Analysis

Used VADER's rule-based sentiment analyzer to calculate a compound score for each cleaned review.

Sentiment labels were assigned using these thresholds:

Positive: compound score ≥ 0.05
Negative: compound score ≤ −0.05
Neutral: compound score between −0.05 and 0.05
4. Exploratory Text Analysis
Calculated frequent words in review text.
Generated a word cloud for reviews rated above 3 stars.
Extracted unigram, bigram, and trigram sequences.
Explored sentiment distributions and category-level patterns.
Results
Dataset size: 1,325,890 reviews retained after preprocessing.
Sentiment pattern: Positive sentiment was the largest category in the reported analysis.
Frequent terms: Words such as book, read, story, love, and great appeared prominently in the analysis.
Visual outputs: Sentiment distribution charts, a word cloud, and word-frequency analysis.

See the notebook and exported charts for the detailed results. Exact sentiment counts and word frequencies should be taken from the final notebook outputs.

Visualizations

Add your exported charts here once available:

Sentiment distribution
Word cloud of highly rated reviews
Most frequent words
Requirements
Python 3
pandas
numpy
nltk
vaderSentiment
matplotlib
seaborn
wordcloud
jupyter
Setup & Usage
Clone or download this repository.
Download the dataset from Kaggle and place the required CSV files in the data/ directory.
Install the dependencies:
pip install -r requirements.txt

Open the notebook:
jupyter notebook notebooks/sentiment_analysis.ipynb

Run the notebook cells in order.

Note: Configure the dataset file paths for your local environment before running the notebook. NLTK may also need to download its required language resources.

Limitations & Future Improvements
VADER may struggle with sarcasm, ambiguous language, and book-specific terminology.
Stopword removal and text cleaning may remove useful contextual information.
Compare VADER with transformer-based sentiment models such as BERT or RoBERTa.
Explore sentiment patterns by book category.
Build an interactive dashboard to make the findings easier to explore.
Skills Demonstrated

Python · Data Cleaning · Exploratory Data Analysis · Natural Language Processing · Sentiment Analysis · Text Analytics · Data Visualization
