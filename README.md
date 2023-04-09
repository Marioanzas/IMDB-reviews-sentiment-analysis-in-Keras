# IMDB-reviews-sentiment-analysis-in-Keras
In this project, I will analyse a dataset from IMDB and use it to predict the sentiment analysis of a review.
I will load the [IMDB dataset](https://ai.stanford.edu/~amaas/data/sentiment/).

This is a dataset of 25,000 movies reviews from IMDB, labeled by sentiment (positive/negative). Reviews have been preprocessed, and each review is encoded as a list of word indexes (integers). For convenience, words are indexed by overall frequency in the dataset, so that for instance the integer "3" encodes the 3rd most frequent word in the data. This allows for quick filtering operations such as: "only consider the top 10,000 most common words, but eliminate the top 20 most common words".
As a convention, "0" does not stand for a specific word, but instead is used to encode the pad token.

In order to do the analysis analysis, a neural network is trained to predict the sentiment of a review based on the words in the review. This is an example of a binary classification problem, an important and widely applicable kind of machine learning problem.