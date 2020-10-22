---
layout: post
title: Video Game Genre Predictor

cover-img: 
thumbnail-img: 
share-img: 
tags: [python, datascience, buildweek, video games]
---
# About the Data
The data set I used contains information about most all video
games released (that sold at least 100,000 copies) from the years 1980
to late 2016 (possibly early 2017).

# What I'm Trying to Do
I'm trying to make a model that can accurately predict
the genre of a video game based on it's publisher, the year it was made,
the platform it was released on, and how well it sold
in different parts of the world. A good (and probably obvious) question this would answer is:
Do these things influence or somehow correlate with the genre of a game?

# How I Went About It
I made a 2 models: a linear model and an XGBoost model. There are 12 different genres, so high accuracy is not easy to acheive. Action is the most frequently occuring genre, but even if you just guess Action every time, you'd only be right 19.89% of the time.

My linear model wasn't much better. It was right 20.69% of the time when I tested it on my validation data and 20.02% accurate on the data it was trained on (notice that it actually performed better on the validation (guessing) data than it did on the training (already known) data). On the other hand, my XGBoost model was able to perform much better than the baseline and linear models! My XGBoost model was able to guess the genre correctly 34.52% of the time on the validation data, and 44.14% of the time on the data it was trained on.

# Results
I know that it doesn't seem like a lot if my model can only guess right 35% of the time, but a jump in roughly 15% accuracy from just guessing Action every time shows that there is a least something there! There is at least a small correlation between the mentioned features (platform, international sales, year released, and publisher) and what genre the particular game is. I was even able to calculate which features played the biggest roles in helping my XGBoost model make each guess! Here's a fun chart of the features from most helpful to least helpful in making each guess:

![Permutation Importance Chart showing weights of each feature.](/assets/img/permuation_importance_chart.png)

