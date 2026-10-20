# Amazon Book Reviews Sentiment Analysis

A Python NLP project analyzing **1.3M+ Amazon book reviews** to identify customer sentiment, frequently used words, and review patterns using Python, Pandas, NLTK, and VADER.

## Project Overview

Customer reviews provide valuable insights into reader preferences and satisfaction. This project applies Natural Language Processing (NLP) and exploratory data analysis to understand sentiment in Amazon book reviews.

The workflow combines data cleaning, text preprocessing, sentiment classification, exploratory text analysis, and data visualization to transform unstructured review text into meaningful insights.

## Key Skills

- Python
- Pandas and NumPy
- Natural Language Processing (NLP)
- Sentiment Analysis
- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- Text Mining and N-gram Analysis
- Data Visualization

## Key Highlights

- Processed **1.3M+ Amazon book reviews**, retaining **1,325,890 records** after removing duplicates and missing values.
- Combined review data with book metadata using Pandas.
- Applied text preprocessing using regular expressions and NLTK stopwords.
- Classified reviews as **positive, negative, or neutral** using VADER.
- Identified the 20 most frequently occurring words in customer reviews.
- Generated a word cloud using reviews rated above 3 stars.
- Extracted unigrams, bigrams, and trigrams to explore common words and phrases.
- Visualized book genre distributions and sentiment patterns across categories.

## Research Questions

- Which words appear most frequently in book reviews rated above 3 stars?
- What is the distribution of positive, negative, and neutral sentiment?
- How does sentiment vary across book categories?

## Dataset

The project uses an **Amazon Book Reviews dataset from Kaggle**, containing customer reviews, book ratings, titles, authors, categories, and related metadata.

The analysis uses two datasets:

- `Books_rating.csv` — Customer reviews, ratings, and review metadata.
- `books_data.csv` — Book titles, authors, categories, and related metadata.

### Features Used

| Feature | Description |
|---|---|
| `Title` | Book title |
| `review/score` | Customer rating of the book |
| `review/text` | Written customer review |
| `authors` | Book author information |
| `categories` | Book category or genre |
| `ratingsCount` | Rating-count metadata |

The original dataset is not included in this repository because of its size. Download both CSV files from the original Kaggle source before running the notebook.

**Dataset Source:** [Amazon Book Reviews Dataset on Kaggle](<YOUR-KAGGLE-DATASET-URL>)

## Project Structure

```text
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
    ├── frequent_words.png
    ├── genre_distribution.png
    └── category_sentiment.png
README.md — Project documentation and setup instructions.

requirements.txt — Required Python dependencies.

.gitignore — Files and directories excluded from version control.

notebooks/ — Jupyter notebook containing the analysis.

data/ — Instructions for downloading and preparing the dataset.

images/ — Exported charts and visualizations.

Note: The dataset CSV files are not included in the repository. The chart filenames listed above should match the images you actually export.

Analysis Workflow
1. Data Preparation
Merged review data with book metadata using book titles.

Selected relevant review and book attributes.

Removed duplicate records and rows containing missing values.

Retained 1,325,890 reviews after preprocessing.

Calculated review word counts.

2. Text Preprocessing
Converted review text to lowercase.

Removed URLs, punctuation, special characters, and numeric terms.

Removed English stopwords using NLTK.

Created a cleaned text column named Clean_Text.

3. Sentiment Analysis
Applied VADER (Valence Aware Dictionary and sEntiment Reasoner), a lexicon-based sentiment analysis tool, to calculate compound sentiment scores for cleaned reviews.

Reviews were classified into three sentiment categories using the following thresholds:

Sentiment

Compound Score

Positive

>= 0.05

Neutral

> -0.05 and < 0.05

Negative

<= -0.05

4. Exploratory Text Analysis
Identified the 20 most frequent words.

Generated a word cloud for reviews rated above 3 stars.

Extracted unigrams, bigrams, and trigrams.

Examined book genre distributions.

Explored sentiment patterns across book categories.

Visualizations
The following visualizations can be exported from the notebook and saved in the images/ directory.

Sentiment Distribution
Shows the distribution of positive, negative, and neutral reviews.

Word Cloud
Highlights frequently occurring words in reviews rated above 3 stars.

Frequent Words
Displays the most frequently occurring words in customer reviews.

Genre Distribution
Illustrates the distribution of books across selected categories.

Sentiment by Category
Compares sentiment counts across book categories.

Key Findings
Positive sentiment was the largest category in the analyzed dataset.

Frequently occurring words included terms such as book, read, story, good, and love.

Word-frequency analysis helped identify recurring themes in highly rated reviews.

Sentiment visualizations provided an overview of customer opinions.

Category-based analysis enabled exploration of sentiment patterns across book genres.

Refer to the notebook's calculated results and visualizations for exact sentiment counts and distributions.

Technologies Used
Python — Core programming language.

Pandas and NumPy — Data manipulation and analysis.

NLTK — Natural language processing and stopword removal.

VADER — Lexicon-based sentiment analysis.

Regular Expressions (Regex) — Text cleaning and pattern matching.

Matplotlib and Seaborn — Data visualization.

WordCloud — Word cloud generation.

Jupyter Notebook — Interactive analysis and experimentation.

Getting Started
Prerequisites
Python 3.9 or later

pip

Jupyter Notebook

Amazon book reviews dataset

Installation
1. Clone the repository


bash
git clone <YOUR-REPOSITORY-URL>
cd amazon-book-reviews-sentiment-analysis
2. Create a virtual environment


bash
python -m venv .venv
3. Activate the virtual environment

Windows:


bash
.venv\Scripts\activate
macOS or Linux:


bash
source .venv/bin/activate
4. Install dependencies


bash
pip install -r requirements.txt
5. Download the dataset

Download Books_rating.csv and books_data.csv from the Kaggle source linked above.

Place both files in the data/ directory and update the notebook file paths if necessary.

6. Launch Jupyter Notebook


bash
jupyter notebook
Open notebooks/sentiment_analysis.ipynb and execute the cells to reproduce the analysis.

Limitations
VADER may struggle with sarcasm, contextual meaning, and domain-specific language.

Processing large datasets can require substantial memory and computation time.

Removing punctuation and stopwords may discard useful contextual information.

Sentiment classifications are lexicon-based predictions and may not always match the reviewer's intended meaning.

Future Improvements
Compare VADER with machine learning and transformer-based sentiment models.

Evaluate sentiment predictions against manually labeled reviews.

Apply topic modeling to identify recurring themes in book reviews.

Develop an interactive dashboard to explore sentiment by book category.

Optimize text preprocessing and sentiment analysis for large datasets.

References
Hutto, C. J., & Gilbert, E. (2014). VADER: A Parsimonious Rule-Based Model for Sentiment Analysis of Social Media Text. Proceedings of the International AAAI Conference on Web and Social Media.

Kaggle — Amazon Book Reviews Dataset. See the dataset link above.
