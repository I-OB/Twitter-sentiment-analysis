# Twitter-sentiment-analysis

## Overview
The purpose of this sentiment analysis of Twitter data related to four popular tennis players, Federer, Djokovic, Nadal, and Tsitsipas. People post real time messages about their opinions on these players. The analysis will help us understand the overall sentiment expressed on Twitter towards these players during a specific period from 31st May of 2021 until 6th June of 2021. The chosen period is right after Roland Garros, one of the biggest yearly tournaments in tennis, where interest is growing. With the use of machine learning to understand whether the sentiment of a tweet is positive, neutral or negative.

### Keywords
Sentiment Analysis, Machine Learning, Twitter Scraping, Pandas, Workcloud, MySQl Database, Snscrape

## Table of Contents
1. [Methodology](#Methodology)
2. [Dataset](#Dataset)
3. [Database](#Database)
4. [Conclusion-Findings](#Conclusion-Findings)

## 1. Methodology <a name="Methodology"></a>

To acquire data for the sentiment analysis project, there was an initial attempt to utilize Twitter's API. However, encountering difficulties in obtaining access, an alternative approach was sought to collect Twitter data without API integration. This was accomplished using the Python package called snscrape. The necessary packages, namely snscrape and pandas, were installed to facilitate the data collection process.  To systematically organize and manage the collected data, a MySQL database table was established. The sentiment classification of the tweets was performed using the TextBlob library.

## 2. Dataset <a name="Dataset"></a>
Subsequently, a Python script was developed to extract 1000 tweets related to the specified query, focusing exclusively on English language content. The information gathered encompassed user details, user followers, tweet counts per user, retweet counts per user, associated hashtags, tweet dates, user locations (where available), and the actual text of each tweet.

## 3. Database <a name="Database"></a>
To systematically organize and manage the collected data, a MySQL database table was established. The sentiment classification of the tweets was performed using the TextBlob library.

## 3. Conclusion-Findings <a name="Conclusion-Findings"></a>
* 22 tweets (2,2%) were duplicate texts. Those tweets are almost certainly from bots or automated accounts.
* More than 60% of the tweets are positive even though we think social media is often a place of critique and hate.
* 690 tweets were mentioning only one athlete, while 277 tweets were mentioning more than one athlete. We can assume that people mainly coming to tweeter to comment positive (as we saw in our graphs) about their favorite athlete.
* Very little people are giving their location, which we assume is for privacy reasons.
* About 85% people are using hashtags on their tweets.
* Even though we set the query to extract the tweets in the span of a month we get our 1000 tweets in less than 24 hours. People are commenting constantly about those athletes.
