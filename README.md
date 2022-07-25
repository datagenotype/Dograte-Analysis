# Dograte-Analysis

## Data wrangling process
The aim of the project is to put the data wrangling skill into practice. Three datasets were used for this project using different libraries from python such as request, Tweepy and pandas. The request was used to extarct data from HTML, tweepy was used to extract data from tweeter while pandas was used to get data from a csv file. After the extraction of data from twitter, The data was programmed into a j_son file. The followings are the libraries used for this project: import tweepy from tweepy import OAuthHandler import json from timeit import default_timer as timer import pandas as pd import requests import numpy as np from functools import reduce import re import seaborn as sns import matplotlib.pyplot as plt.

After the data gathering had been manifested, ,I assesed the dataset one after the other programmatically and visually. These are the quality and tidiness issues I found:

Data columns like in_reply_to_status_id,in_reply_to_user_id,retweeted_status_id,retweeted_status_user_id have a lot of missing data and as a result of this they will be dropped. They are also not relevant for this analysis.

The data in source column needs to be clean

There are outliers in the rating_numerator which has the minimum and maximum 1 and 1776 respectively.

In the rating_denominator column, 10 should be expected to be seen but we have outliers like 0 and 170.

The column 'name' has some strange object like a,an,such,etc.

The data type for timestamp sould be in datetime not in string format and tweed_id should be in string.

Renaming some columns like so as to be more descriptive

Some variables that are not wanted in the analysis will be dropped.

doggo, floffer, pupper and pupo should be grouped in a column called 'stage'

The three dataset need to be merged

## Conclusion
After the whole cleaning, i stored the cleaned and merged dataset into a csv file called twitter_archive_master.csv. after that, I was able to deduce insights from the analysis and they are :


Favorite and retweet counts are highly positively correlated.

It can be deduced from the above analysis that the pupper has the highest frequency or occurence.

It can be seen that floofer has the highest rating compared to other dog stage
