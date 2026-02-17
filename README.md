 DATA 622 – Homework 2
 Natural Language Processing (NLP) Pipeline
 Project Overview

This project is part of the DATA 622 – Machine Learning course and focuses on building a basic NLP preprocessing pipeline using Python. The task involves extracting textual content from a web article and applying multiple NLP techniques such as cleaning, normalization, stopword removal, and lemmatization.

The goal is to understand how raw textual data is transformed into a structured format suitable for machine learning models.

 Objectives

Extract text data from a given URL

Clean and preprocess text data

Apply NLP techniques using NLTK

Compare lemmatization vs stemming

 Problem Statement

Perform the following steps on the given article:

Read the file

Extract the content from the provided CNN article

Print the first 700 characters

Remove HTML Tags

Clean the text by removing HTML elements

Lowercase & Remove Punctuation

Convert all text to lowercase

Remove punctuation symbols

Remove Stopwords

Use NLTK’s English stopwords

Filter out unnecessary words

Lemmatization

Apply WordNetLemmatizer

Print first 50 lemmatized words

Analysis Task

Compare results with stemming

Identify differences in output

 Technologies Used

Python 3.x

NLTK (Natural Language Toolkit)

Requests / BeautifulSoup (for web scraping)

Regular Expressions (re)

 Project Structure
DATA-622-Homework-2/
│
├── homework2.ipynb      # Main notebook / script
├── requirements.txt     # Dependencies
└── README.md            # Project documentation


 Installation
 
Clone the repository:

git clone https://github.com/your-username/DATA-622-Homework-2.git
cd DATA-622-Homework-2


Install dependencies:

pip install -r requirements.txt


Download NLTK resources:

import nltk
nltk.download('stopwords')
nltk.download('punkt')
nltk.download('wordnet')

 Implementation Steps
1. Read Web Content

Fetch HTML from the given URL

Extract raw text

2. Clean Text

Remove HTML tags using BeautifulSoup

Normalize text

3. Preprocessing

Convert to lowercase

Remove punctuation

4. Stopword Removal

Use NLTK stopwords

Filter tokens

5. Lemmatization

Use WordNetLemmatizer

Convert words to base form

6. Stemming Comparison

Use PorterStemmer

Compare output differences

 Sample Output
First 700 characters:
"luxury brands are expensive because..."

First 50 lemmatized words:
['luxury', 'brand', 'expensive', 'consumer', 'market', ...]

Stemming Output:
['luxuri', 'brand', 'expens', 'consum', 'market']

 Lemmatization vs Stemming
Aspect	Lemmatization	Stemming
Output	Meaningful words	Root fragments
Accuracy	High	Medium
Speed	Slower	Faster
Example	"running" → "run"	"running" → "run" / "runn"
Conclusion:

Lemmatization produces human-readable words

Stemming is faster but less accurate

 Key Learnings

Importance of text preprocessing in NLP

Difference between clean vs raw text

Trade-offs between lemmatization and stemming

Handling real-world web data

 Future Enhancements

Add TF-IDF / Bag-of-Words

Perform sentiment analysis

Build a classification model

Use spaCy for advanced NLP
