# Analyzing WeRateDogs Twitter archive

## Date created
This project was created on 2021-03-27.

## Description

This project aims to gather, clean and analyze data from [WeRateDogs Twitter archive](https://twitter.com/dog_rates).
WeRateDogs is a twitter profile that posts pictures of dogs with a funny description. It has over 8.9M followers and it got famous with its creative rating system where the denominator is almost always 10 but the numerator is usually superior to 10. 

This work was made to complete an assignement for the [Udacity Data Analyst Nanodegree](https://www.udacity.com/course/data-analyst-nanodegree--nd002).

## Files used

`wrangle_act.ipynb` : a jupyter notebook for gathering, cleaning, and analyzing the data. 

`twitter-archive-enhanced.csv` : a file that contains basic tweet information (twitter IDs, text, timestamp...) of +5000 tweets, courtesy of [WeRateDogs](https://twitter.com/dog_rates).

`tweet_json.txt` : a file containing additional information (retweet count, favorite count, ...) about the tweets of `twitter-archive-enhanced.csv` formatted as JSON. This file was created by querying the Twitter API using the tweet IDs. You can either use it directly or create it yourself by running the code cells for downloading the data but you will need to set up a Twitter app to gain access tokens.

`image_predictions.tsv` : a file provided by Udacity that contains dogs' breed predictions based on the tweet's image. You can use the file directly or download it programmatically with the dedicated code cell.

`twitter_archive_master.csv` : the clean data file that was used for the analysis. 

`wrangle_report.pdf` : a report outlining the main steps of gathering, assessing, and cleaning the data. 

`act_report.pdf` : a report of the results of the analysis. 

## Installation

To run the notebook, you will need `python`, `numpy`, `pandas`, `matplotlib`, and `seaborn` installed. If you want to run the cells for downloading the data from Twitter, you will need to create a Twitter app and install `tweepy` for querying the API. 

You can install all these libraries (except `tweepy`) individually or with [Anaconda](https://www.anaconda.com/), a python distribution with a focus on data science. If you’re interested in Anaconda you can follow their [installation guide](https://www.anaconda.com/distribution/).

To create your Twitter app, you will firstly need to sign up for a [Twitter Developper Account](https://developer.twitter.com). You will be asked to fill in basic profile information and give a detailed description of how you're going to use their API. You have to be as specific as possible. After sending your application, it will be reviewed and you will receive their response in the email that you registered with. You can have a positive answer, a negative one or they will ask you to send them an email with additional information. In that case, you should copy their email and put your answers directly below their questions. This process can take quite some time. For this project, it took 3 emails over one week to get approval. If you're not interested in running the cells for downloading the data or if they refuse your application, you can use `tweet_json.txt`.  

After getting your access tokens, you can start using [Tweepy](https://www.tweepy.org/). It is an easy-to-use library for accessing the Twitter API. It was used in this project to create `tweet_json.txt`. You can install it using the command below:

`pip install tweepy`


