# Naive Bayes

A simple but powerful classification algorithm based on 
probability. Especially popular for text classification.

## Why "Naive"?
It assumes all features are completely independent of 
each other. In reality this is often not true — but 
despite this naive assumption it works surprisingly 
well in practice.

## Simple analogy:
You receive an email with the words "FREE MONEY."
From past experience you know 90% of emails with 
these words were spam. So you think — probably spam.
That's Naive Bayes — using past experience to calculate 
the probability of each class.

## How it works:
Training:
- Calculate probability of each word appearing in spam
- Calculate probability of each word appearing in normal emails

Prediction:
- For a new email calculate probability of spam vs not spam
- Whichever probability is higher wins

## TF-IDF connection:
TF-IDF converts text into numbers representing word importance.
- TF (Term Frequency) — how often a word appears in the document
- IDF (Inverse Document Frequency) — how rare the word is overall
Common words like "the" get low scores.
Rare meaningful words like "winner" get high scores.
These numbers become the features Naive Bayes uses.

## Advantages:
- Very fast to train and predict
- Works extremely well for text classification
- Works well even with small amounts of data

## Disadvantages:
- Independence assumption is often wrong
- Not great for complex relationships in data

## Real world examples:
- Spam email detection
- Sentiment analysis — positive or negative review
- Document categorization — sports, politics, entertainment
- Medical diagnosis
