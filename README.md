# IMDB Sentiment Prediction



## Overview

IMDb is one of the largest(if not, *the largest*) movie, film, and television databases in the world. IMDb collects information relevant to nearly every movie ever filmed, including cast, production crew, plot summaries, trivia, ratings, critic reviews, and fan reviews.<sup>1</sup> 

Critic and fan reviews are often given a star rating or a rating out of 10, but additional(richer) information is contained in how any particular reviewer either talks or writes about their experience watching a show. With the rise of deep learning and Natural Language models we have the ability to analyse the sentiment within a review, potentially giving us a deeper insight into how the viewer actually felt about their viewing experience.



*The goal of this project is to build a model which can predict whether the written review for a movie is positive or negative.*



## Data

Link to Dataset: https://www.kaggle.com/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews

* Balanced (equal amount of positive and negative reviews)
* No missing data (only needs pre-processing)
* Data Split 10% train/90% test
* 49581 samples total



## Model Used

* BERT (pretrained from HuggingFace library)



## Results

F1-score: 0.88



## Techniques Used

* Transfer learning (using pretrained model from HuggingFace)
* Preprocessing steps used:
  * Removed:
    * HTML tags
    * Emojis
    * Punctuation & Special Characters
    * Accented characters
    * URLs
  * Expand contractions
  * Make all text lowercase



## Potential Improvements

* Try other models (eg. GPT-2, RoBERTa, or DistilBERT)
* Ensemble different models
* Use a K-Fold Ensemble
* Train on more data (20/80 split instead of 10/90 split)
* Pre-train on a different task(eg. next word prediction)
* Use learning rate finder and learning rate scheduler



##### References

1. https://en.wikipedia.org/wiki/IMDb 
