_**Spam Email Classifier**_

A machine learning pipeline to classify emails as spam or ham (non-spam) using a bag-of-words + classifier approach.

_**Project Overview**_

This project builds a text classification system to distinguish spam emails from ham (legitimate) emails. It uses a dataset of labeled email messages (spam vs. not spam) and applies standard text preprocessing, vectorization, and classification algorithms to build a predictive model.

_**Features**_
Text preprocessing (cleaning, tokenization, stopword removal, etc.)

Vectorization using CountVectorizer or TF-IDF

Use of sklearn Pipeline and ColumnTransformer for clean workflows

Multiple classification algorithms (e.g. Naive Bayes, Logistic Regression)

Model evaluation using metrics such as accuracy, precision, recall, F1-score, confusion matrix

Ability to predict on new/unseen emails

**Repository Structure**__
.

├── README.md

├── Spamemailclassifier.ipynb     ← main Jupyter Notebook

├── requirements.txt              ← Python dependencies  

├── spam.csv                       ← dataset  
