Amazon Book Reviews Sentiment Analysis

A data analytics and NLP project analyzing 1.3M+ Amazon book reviews using Python, Pandas, NLTK, and VADER to identify customer sentiment and review patterns.

Project Overview

Customer reviews provide valuable insights into product satisfaction and customer preferences. This project processes Amazon book reviews to classify customer sentiment, identify frequently used words, and explore differences across book categories.

Key Highlights
Processed 1.3M+ book reviews after removing duplicate and missing records.
Built a text preprocessing workflow using Python, Pandas, regular expressions, and NLTK.
Applied VADER to classify reviews as positive, negative, or neutral.
Analyzed frequently occurring words and generated word cloud visualizations.
Explored sentiment distributions and relationships between book categories and sentiment.
Business Questions
What words appear most frequently in highly rated book reviews?
What proportion of reviews express positive, negative, or neutral sentiment?
How does customer sentiment vary across book categories?
Results
Dataset: 1,325,890 reviews retained after preprocessing.
Sentiment: Positive reviews formed the largest sentiment category in the reported analysis.
Review insights: Frequently occurring words included book, read, story, love, and great.
Visual analytics: Created sentiment distribution charts, word clouds, and category-level comparisons.

See the notebook and visualizations for the detailed analysis. Reported word frequencies and sentiment counts should be verified against the final notebook outputs.

Tools & Technologies
Language: Python
Data Analysis: Pandas, NumPy
NLP: NLTK, VADER Sentiment Analysis
Visualization: Matplotlib, Seaborn, WordCloud
Environment: Jupyter Notebook
Workflow
Load and combine book review and book metadata datasets.
Remove duplicate records and handle missing values.
Clean and normalize review text.
Calculate VADER compound sentiment scores.
Classify reviews into positive, negative, and neutral categories.
Analyze word frequencies and visualize sentiment patterns.
Getting Started
1. Install dependencies
pip install -r requirements.txt

2. Download the dataset

Download the original Amazon book reviews dataset from Kaggle.

The dataset is not included in this repository because of its size.

3. Run the notebook

Open notebooks/sentiment_analysis.ipynb in Jupyter Notebook and configure the dataset file paths before running the analysis.

Limitations & Future Improvements
VADER may struggle with sarcasm, ambiguous language, and book-specific terminology.
Compare VADER predictions with transformer-based models such as BERT.
Build an interactive dashboard to explore sentiment by category.
Improve reproducibility through configurable data paths and automated preprocessing.
Skills Demonstrated

Python · Data Cleaning · Exploratory Data Analysis · Natural Language Processing · Sentiment Analysis · Data Visualization · Text Analytics

Your Name

GitHub · LinkedIn
