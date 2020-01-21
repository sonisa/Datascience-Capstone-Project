Data science capstone Presentation
========================================================
author: Sonisa Sharma
date: 1-20-2019
autosize: true
* [Next Word Prediction Shiny App](https://sonisa56.shinyapps.io/data/)
* [GitHub url](https://github.com/sonisa/Datascience-Capstone-Project)

Predict the Next word

1. Introduction
========================================================
The goal of this exercise is to create a product to highlight the prediction algorithm that you have built and to provide an interface that can be accessed by others. 

2. Text Preprocess and n-grams
========================================================
### 2.1 DATA:

The dataset for this word prediction app was gathered from three sources:

* Blogs
* News
* Twitter

Data was preprocessed and tokenized with *quanteda* library.

Slide With Code
========================================================

The code for this project is at [github repo] at "https://github.com/sonisa/Datascience-Capstone-Project"

Processing of Data
========================================================

A subset of the original data was sampled from the three sources (blogs,twitter and news) which is then merged into one.
Next, data cleaning is done by conversion to lowercase, strip white space, and removing punctuation and numbers.
The corresponding n-grams are then created (Quadgram,Trigram and Bigram).
Next, the term-count tables are extracted from the N-Grams and sorted according to the frequency in descending order.
Lastly, the n-gram objects are saved as R-Compressed files (.RData files).
