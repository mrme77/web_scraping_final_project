# Project Title

Module 7 Final Project: Web Scraping

## Description
This project is part of the Web Mining and Applied NLP (44-620) course, student's name is Pasquale Salomone. The notebook aims at scraping a website to retrive some uself information and create effective visualizations.Here is the link to the Github repository: https://github.com/mrme77/web_scraping_final_project.

## Table of contents

### Scraping data from url
The code in this section attempts to access the url https://www.euronews.com/2023/07/18/disloyal-views-lithuania-strips-russians-residency-permits" 
and create a Beautifulsoup response with the article text.

### Data processing with Spacy module
Read in the contents of the Beautifulsoup object, and creates a nlp pipeline with Spacy library.

### Sentiment Analysis
This section of the notebook performs sentiment analysis. In specific, it focuses on polarity score, the sentiment polarity of the text, and subjectivity score which is the subjectivity of the text.

### Top 5 recurring words from the article
After removing white space, punctuation, and stop words, this section attempt to find the top 5 recurring word leveraging the Counter class from the collections module

### Word cloud from the article's words
This createa wordcloud visualization with the pre-processed article data.

### Distribution of common words in the article's sentences
Creates a function that takes a sentence and a list of interesting tokens and returns the number of times that any of the interesting words appear in the sentence divided by the number of words in the sentence.

### Summarize the article with one sentence
This section attempts to summarize the processed article in one sentence. It leverages the sumy library and some of its classes.

## Installation

To use this project, make sure you have Python 3.8 installed on your system. Do not install modules like math and statistics. You can check your Python version by running the following command in your terminal:

```shell
python --version
```

### Modules

The following modules are required for the installation of this project:
<br>
```
from bs4 import BeautifulSoup
from wordcloud import WordCloud
import json,pickle,requests,spacy,re,nltk
from spacytextblob.spacytextblob import SpacyTextBlob
from spacy.lang.en.stop_words import STOP_WORDS
import matplotlib.pyplot as plt
from collections import Counter
from sumy.parsers.html import HtmlParser
from sumy.nlp.tokenizers import Tokenizer
from sumy.summarizers.lex_rank import LexRankSummarizer
from nltk.tokenize import sent_tokenize
import numpy as np
nltk.download('punkt')
```

## Acknowledgments

I would like to acknowledge the following resources that were instrumental in the development of this project:

- ChatGPT by OpenAI: We used ChatGPT, a powerful language model, to assist in generating responses and providing guidance during the development process. ChatGPT played a crucial role in enhancing the functionality and accuracy of our project.

- Stack Overflow: We would like to express our gratitude to the vibrant community of developers on Stack Overflow. Their valuable insights, code snippets, and solutions to various programming challenges have been immensely helpful in solving problems encountered during the development of this project.
