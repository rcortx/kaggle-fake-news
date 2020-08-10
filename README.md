# kaggle-fake-news
Baseline TFIDF solution to https://www.kaggle.com/c/fake-news/data


Classifier uses a basic Text processing pipeline over just the `text` column to predict fake news:

1. Text cleaning: accent removal, lower case
2. Tokenization
3. Stopword removal
3. Lemmatization/Stemming
4. TFIDF vectorization
5. Experiments with tree classifiers like Decision Trees and Gradient Boosted Trees
6. Achieved F1 of 87-91.5% on 20% validation set (best F1 with Gradient Boosted Trees) (NOTE: this is not k-cross validated)


Next Steps:

1. Use other columns to improve classifier performance like `author`, `title`, etc
2. Use BERT based vectorization instead of TFIDF
