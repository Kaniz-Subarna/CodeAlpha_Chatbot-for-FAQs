# Chatbot for FAQs 

This project is a FAQ Chatbot designed to answer user questions related to a specific topic or product. The chatbot uses Natural Language Processing (NLP) techniques to preprocess text, match user queries with the most relevant FAQ, and return appropriate answers.

The chatbot also features a visual, centered interface in Google Colab, where users can type questions and receive answers inside a single, professional-looking chat box. This makes it ideal for business demos, product FAQs, or educational purposes.

[Note: Here I use some common FAQS from a Skincare Product business.]


## Features

- Collect and store FAQs for a topic or product.
- Preprocess text using NLP techniques:
- Tokenization
- Lowercasing
- Stopword removal
- Match user queries with the most similar FAQ using TF-IDF vectorization and cosine similarity.
- Display answers in a modern, centered chat interface.
- Supports both business and customer perspective FAQs.
- Fully interactive in Google Colab, no external deployment required.


## Technology Use

- Python 3
- NLTK (Natural Language Toolkit) – for text preprocessing
- Scikit-learn – for TF-IDF vectorization and cosine similarity
- Ipywidgets – for creating a visual chat interface in Colab
- HTML & CSS – for styling and centering the chatbot interface


## Installation

1. Install Dependencies
```bash
pip install nltk scikit-learn ipywidgets
```

2. Download NLTK Data

```bash
import nltk
nltk.download('punkt')
nltk.download('stopwords')
```


3. Run the Notebook

- Open the ``` FAQ_Chatbot.ipynb ``` file in Google Colab.
- Run all cells sequentially.
- The centered chat interface will appear, where you can type questions and get responses immediately.

    
## How It Work
- Collect FAQs – A Python dictionary stores questions and answers.
- Preprocess Questions – User input and FAQ questions are preprocessed:
- Convert text to lowercase
- Remove punctuation
- Tokenize words
- Remove stopwords
- TF-IDF Vectorization – Converts questions into numerical vectors.
- Similarity Matching – Compares user input vector with FAQ vectors using cosine similarity to find the best match.
- Chat Interface – Displays both user questions and chatbot answers in a single centered box.

## Usage
- Type your question in the input box.
- Click the Ask button.
- The chatbot will display the most relevant answer from the FAQ list inside the chat box.
- Scroll to view previous interactions.
## Authors

- [@Kaniz-Subarna](https://www.github.com/Kaniz-Subarna)
