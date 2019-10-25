# reddit-binary-classifier

## Problem Statement
The participation rate at a local church have been declining over the years. The church committee would like to reconnect with the Christian community by emailing event updates to existing and occasional churchgoers. The committee have approached us to build a system that is able to identify Christians from their online posts as they do not want to hard sell on atheists.

## Executive summary
This is a classification problem where we will build a model that is able to identify Christians from atheists based on their online posts. As reddit has a big community for both Christians and atheists, we will scape reddit for the two topics and train a binary classifier that will classify which group a poster is from based on their text input

Steps in building the system:


3  Scraping for data

4  Read the csv file

5  EDA: Exploring the dataset

5.1  Word Cloud visualization for dataset

6  Feature Engineering : Train test split

6.1  Creating X and y

6.2  Baseline accuracy

7  NLP Pipeline

7.1  Tokenizing, Stemming/Lemming and Vectorization

7.2  Model 1 : Count Vectorizer - Logistic Regression

7.3  Model 2 : Count Vectorizer - Lemmatizer - Logistic Regression

7.3.1  Scores and best parameters obtained from Grid Search based on this dataset is:

7.4  Model 3 : Count Vectorizer - Porter Stemmer - Logistic Regression

7.5  Model 4 : Count Vectorizer - Lemmatizer - Multinomial Naive Bayes

7.6  Model 5 : TF-IDF - Lemmatizer - Multinomial Naive Bayes

7.7  Model 6 : TF-IDF - Lemmatizer - Multinomial Naive Bayes Model 2

7.7.1  Intepreting Model 4

7.8  Model 5 : Gradient Boosting Classifier
8  Model Benchmarks
8.1  Optimizing for Recall
8.2  Plotting the AUC ROC Curve of the best model
8.3  Plotting the distribution of probabilities
9  Visualizing the most frequent words in each subreddit
10  Export the best Model
11  Running the final model on Test set
12  Conclusion
