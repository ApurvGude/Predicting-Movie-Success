# Predicting-Movie-Success

Over the past decade, Bollywood cinema has witnessed exponential growth in terms of movies released, number of people employed and profits earned. 

Hence a model to predict whether a movie will be a success or not in the box office before release will prove to be highly useful to everybody involved.

In this project, we have been provided with data of about 1300 movies which released from 2001-2014. All these movies have been ranked from 1 to 9 on the basis of their success with 9 being an all-time blockbuster and 1 being a disaster.

The dataset has been obtained from [Kaggle](https://www.kaggle.com/mitesh58/bollywood-movie-dataset) and from other sites like boxofficeindia.com and IMDB.

With each movie, we are given its release information,genre, actors, writers and directors involved. For each actor and director ,their previous movie ratings and current success has also been provided.

The hitFlop column contains values from 1 to 9 with
1. - Disaster
2. - Flop
3. - Below Average
4. - Average
5. - Semi Hit
6. - Hit
7. - Super Hit
8. - Blockbuster
9. - All-Time Blockbuster

## [Part 1: Data Exploration and Wrangling](https://github.com/ApurvGude/Predicting-Movie-Success/blob/master/notebooks/Data%20Exploration%20and%20Wrangling.ipynb)

![Image 1](https://github.com/ApurvGude/Predicting-Movie-Success/blob/master/images/image1.png)

In this section we go through all the columns of each dataset and try to figure out which features play a huge role in a movie being a success. We also analyze relations between features by making different types of graphs.

We also transformed all useful features from each dataset to a a final dataset which can be used for predictions.

Based on the analysis we found out that the most important features were the actors and directors current popularity and the succes of their previous movies.

## [Part 2: Creating the Classification Model](https://github.com/ApurvGude/Predicting-Movie-Success/blob/master/notebooks/Making%20the%20classification%20model.ipynb)

We tried out a variety of classifiers of different types - linear,tree,ensemble and others and based on the results we chose ExtraTreesClassifier.

Using this model we were able to obtain a ROC_AUC score of about 0.79.

## [Part 3: Exploring the results and making final observations](https://github.com/ApurvGude/Predicting-Movie-Success/blob/master/notebooks/Analyzing%20Results%20and%20making%20final%20observations.ipynb)

After mmaking the model, we analyzed the final results and even made a confusion matrix for our prediction model. Using the models feature importances ,we also figured out which features were important for predicting success/

We made a prediction model and wrote some final observations based on these predictions. Some ways to improve the model were also given.
