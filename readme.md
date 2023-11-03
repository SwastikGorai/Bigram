# Bigram Model Implementation in Python

This repository contains an implementation of a Bigram Model in Python. There are approx 40,000 names in the `names.txt` file which is used to generate more names using the bigram concept.

## Introduction
A Bigram Model is a statistical language model that is based on the probability of a word given its preceding word. It's a simple but effective way to model the probability of a sequence of words in a text. This implementation provides a straightforward Python code to build and use a Bigram Model for text generation or other natural language processing tasks.

## What is a Bigram Model?
A Bigram Model is a type of probabilistic model that predicts the likelihood of a word given the previous word in a sequence of words. In other words, it models the conditional probability of observing a word given the previous word. The "bi" in "bigram" refers to the fact that it considers pairs of consecutive words.

For example, consider the sentence: `"Chatbots are amazing"`. In terms of bigrams, this sentence can be represented as:

* (START, Chatbots)
* (Chatbots, are)
* (are, amazing)
* (amazing, END)

## How does the Bigram Model Work?
The Bigram Model calculates the probability of a word given the previous word using the following formula:

```
P(word | previous_word) = Count(previous_word, word) / Count(previous_word)
```

Where:

* `Count(previous_word, word)` is the number of times the word word follows the word previous_word.
* `Count(previous_word)` is the number of times the word previous_word occurs in the dataset.
* The model uses these probabilities to generate text or make predictions based on a given context.
