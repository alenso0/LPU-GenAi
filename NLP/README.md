# NLP

Natural Language Processing basics, worked through an SMS spam classification problem.

## What's in here

| Path | Description |
|---|---|
| `NLP_basics.ipynb` | Main notebook — EDA, text cleaning, stopword removal, stemming, word cloud, vectorization (CountVectorizer, TF-IDF), and tokenization/padding for a neural model |
| `nlp-basics.ipynb` | Outline/scratch notebook for the topics covered |
| `spam.csv` | SMS spam/ham dataset used for text classification |
| `twitter_mask4.jpeg` | Mask image used to shape the word cloud |

## GloVe word embeddings

`NLP_basics.ipynb` uses pretrained GloVe vectors (`glove.6B.100d.txt`) for word embeddings. This file is **not committed** to the repo (it's ~350MB and ignored via `.gitignore`).

Download it from Kaggle and place it in this `NLP/` folder before running the embedding cells:

https://www.kaggle.com/datasets/danielwillgeorge/glove6b100dtxt?resource=download

## Running the notebook

```bash
pip install nltk wordcloud
jupyter notebook NLP_basics.ipynb
```

Run cells top to bottom — `nltk.download(...)` calls in the first code cell fetch the stopwords/tokenizer corpora needed later on.
