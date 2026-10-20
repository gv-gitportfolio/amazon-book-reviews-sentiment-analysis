# Amazon Book Reviews Sentiment Analysis

## Project Overview

Analyze **1.3M+ Amazon book reviews** using Python, NLTK, and VADER.

## Key Skills

- Python
- Data Analysis
- Natural Language Processing
- Sentiment Analysis


Amazon Book Reviews Sentiment Analysis
📌 Project Overview

A Python NLP project analyzing 1.3M+ Amazon book reviews to identify customer sentiment, frequently used words, and review patterns using Pandas, NLTK, and VADER.

Customer reviews provide valuable insights into product satisfaction and reader preferences. This project analyzes Amazon book reviews to understand reader sentiment, identify recurring themes, and explore patterns in highly rated reviews.

The workflow combines data cleaning, text preprocessing, sentiment classification, exploratory data analysis, and data visualization to transform unstructured review text into meaningful insights.

🎯 Key Skills
Python
Data Analysis
Natural Language Processing (NLP)
Sentiment Analysis
Data Cleaning and Preprocessing
Exploratory Data Analysis (EDA)
Data Visualization
✨ Key Highlights
Processed 1.3M+ book reviews after removing duplicate and missing records.
Applied text preprocessing using Pandas, regular expressions, and NLTK.
Classified reviews as positive, negative, or neutral using VADER.
Identified frequently occurring words in customer reviews.
Created word clouds and sentiment distribution visualizations.
Explored review patterns across book categories.
❓ Business Questions
Which words appear most frequently in book reviews rated above 3 stars?
What is the distribution of positive, negative, and neutral sentiment?
How does sentiment vary across different book categories?
What recurring themes appear in highly rated book reviews?
📊 Dataset

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

🗂️ Project Structure
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

notebooks/ — Jupyter notebook containing the analysis.
data/ — Instructions for downloading and preparing the dataset.
images/ — Exported charts and visualizations.
requirements.txt — Python dependencies.
.gitignore — Files and directories excluded from version control.

Note: The data/ directory contains dataset instructions rather than the raw CSV files.

⚙️ Analysis Workflow
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

Applied VADER (Valence Aware Dictionary and sEntiment Reasoner), a lexicon-based sentiment analysis tool, to calculate a compound sentiment score for each cleaned review.

Reviews were classified using the following thresholds:

Sentiment	Compound Score
Positive	>= 0.05
Neutral	> -0.05 and < 0.05
Negative	<= -0.05
4. Exploratory Text Analysis
Calculated the most frequently occurring words in review text.
Generated a word cloud for reviews rated above 3 stars.
Examined recurring terms and themes in customer feedback.
Explored sentiment distribution and review patterns across book categories.
📈 Visualizations

The following visualizations can be found in the images/ directory.

Sentiment Distribution

Displays the distribution of positive, negative, and neutral reviews.

!Sentiment Distribution

Word Cloud

Highlights frequently occurring words in book reviews rated above 3 stars.

!Word Cloud

Frequent Words

Shows the most frequently occurring words in the review dataset.

!Frequent Words

🛠️ Technologies Used
Python — Core programming language.
Pandas — Data manipulation and cleaning.
NLTK — Natural language processing and stopword removal.
VADER — Rule-based sentiment classification.
Matplotlib and Seaborn — Data visualization.
WordCloud — Word cloud generation.
Jupyter Notebook — Interactive analysis and experimentation.
🚀 Getting Started
Prerequisites
Python 3.9 or later
pip
Jupyter Notebook
The Amazon book reviews dataset
Installation

1. Clone the repository

git clone <your-repository-url>
cd amazon-book-reviews-sentiment-analysis


2. Create a virtual environment

python -m venv .venv


Activate the environment:

Windows

.venv\Scripts\activate


macOS / Linux

source .venv/bin/activate


3. Install dependencies

pip install -r requirements.txt


4. Download the dataset

Download the dataset from its original Kaggle source and place the required files in the data/ directory. Update the notebook's file paths if necessary.

5. Launch Jupyter Notebook

jupyter notebook


Open notebooks/sentiment_analysis.ipynb and run the analysis cells.

💡 Key Takeaways

This project demonstrates how natural language processing can be applied to large-scale customer review data to:

Understand customer sentiment beyond numerical ratings.
Identify common themes and frequently discussed topics.
Explore patterns in reader feedback.
Turn unstructured text into interpretable insights through data visualization.
🔮 Future Improvements
Compare VADER predictions with a machine learning sentiment classifier.
Evaluate sentiment predictions against customer ratings.
Apply topic modeling to discover recurring themes.
Build an interactive dashboard for exploring sentiment by category.
Optimize preprocessing and sentiment scoring for large datasets.
👤 Author

Your Name

GitHub: Your GitHub Profile
LinkedIn: Your LinkedIn Profile

If you find this project useful, consider giving the repository a ⭐ on GitHub.







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
