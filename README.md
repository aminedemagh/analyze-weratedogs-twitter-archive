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