**Spam Email Classifier**

A machine learning pipeline to classify emails as spam or ham (non-spam) using a bag-of-words + classifier approach.

**🧰 Project Overview**

This project shows how to build a text classification system (spam detector) using:

A dataset (CSV) of labeled emails

Text preprocessing (tokenization, vectorization)

A ColumnTransformer / Pipeline

A classification algorithm (e.g. Multinomial Naive Bayes, Logistic Regression, etc.)

Prediction on new emails

It is built in a Google Colab note

**🧩 How It Works (High-Level)**

Load data
Read a CSV file containing email messages and their labels (spam / not spam).

Preprocessing & Feature Engineering

Use CountVectorizer (or TfidfVectorizer) to convert raw email text into numeric vectors (word counts or tf-idf)

Possibly clean text (lowercasing, removing punctuation, stopwords)

Use a ColumnTransformer (if you have multiple input columns) or directly apply the vectorizer to the “Message” column

Label Encoding
Encode textual labels “spam” / “ham” into numeric labels (e.g. 0, 1) using LabelEncoder.

Model Training
Build a Pipeline that combines the vectorizer (and any other preprocessing steps) and a classification algorithm (e.g. MultinomialNB, LogisticRegression, etc.). Fit on the training data.

Evaluation
Evaluate on a holdout set (test set) using metrics such as accuracy, precision, recall, F1-score, confusion matrix.

Inference / Prediction
Use the trained pipeline to predict new, unseen email messages. For a single message, wrap it in a structure with the correct feature name (e.g. as a DataFrame with column “Message”) before calling .predict().
