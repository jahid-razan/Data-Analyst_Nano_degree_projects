# Data Analyst Nanodegree- Project 4 Data Wrangling

## 1. Background & Objective of the Project

Data is fun to play with when it clean and meaningful insights can be harnessed from it to formulate strategy and make evidence based decision. Easier said than done because- as is the case with most other practical things in life, the world of data too is messy and data rarely comes as clean.

Hence, the job of a data analyst involves a great deal of preprocessing of data which can consume up to 80% of the effort before even start getting meaningful insight from it [1]. Hence, it is very fundamental for a data analyst or data enthusiast to be able to master the skills of gathering, assessing, and cleaning data that are collected from a variety of sources and formats. Also, it is important for somebody who plays with data to be aware of the quality and tidiness issues.

Twitter is one of the most popular social media platforms with more than 100 million users and more than 340 million tweets. It accounts for a 1.6 billion years queries per day. What makes twitter particularly effective is its precision as users are only allowed to use a limited number of characters [2]. Users use Twitter to share interesting items that includes their hobbies, profession, research articles and updates and latest happenings. Hence it can be used as a very effective data source. Also, twitter data can be accesses using API which has been done in this case.

The dataset in this wrangling project has been obtained from the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators are almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because they're good dogs. WeRateDogs has over 4 million followers and has received international media coverage.

The objective of this project is to use Python and its libraries, to gather data from a variety of sources and in a variety of formats, assess its quality and tidiness, then clean it to create interesting and trustworthy analyses and visualizations. Also, at the end of the analysis, the master data set will be saved in the csv format and some insights have been discussed from. The crucial steps of the whole journey will be explained in a way so that the actions can be followed and the results can be reproduced.




## 2. Installations

This project was written in Python, using Jupyter Notebook on Anaconda. The relevant Python packages for this project are as follows:

* pandas
* NumPy
* requests
* tweepy
* json

To follow the steps it is recommended to install Anaconda, a pre-packaged Python distribution that contains all of the necessary libraries and software for this project.



## 3. Dataset


**A.**  The WeRateDogs Twitter archive: twitter_archive_enhanced.csv has been received from the Udacity instructor and downloded.

**B.**  A file (image_predictions.tsv) is hosted on Udacity's servers and has been downloaded programmatically using the Requests library and the specified URL.

**C.**  Using the tweet IDs in the WeRateDogs Twitter archive, query have been made of the Twitter API for each tweet's JSON data using Python's Tweepy library and entire set of JSON data has been stored in a file called tweet_json.txt file.





## 4. File Descriptions

1.  **Wrangle_act_1**: Data have been gather using the sources mentioned in A,B and C

2.  **Wrangle_act_2**: Deals with data quality and tidyness issues of the twitter_archive_enhanced.csv file.

3.  **Wrangle_act_3**: Deals with the data quality and tidyness issues of the image_predictions.tsv file

4.  **Wrangle_act_4**: In this file the data quality and tidyness issues of the twitter data obtained using the API has been dealt. Then all the dataframe has been merged, and the vizualizations have been made.



## 5. Dataset Overview

After cleaning the dataset all the three dataframes have been merged into a df_master file.

### A. What is the structure of this dataset?

The df_master data consists of of 1958 rows and 20 columns. There are 3 boolean variables, 3 floats, 7 integar, and 7 strings. The variables provide information about the name of the dog, time of tweet-day, month, hour, and year, dog stages, p1, p2, p3- the algorithm's #1, #2, #3 prediction for the image in the tweet, p1_conf, p2_conf, p3_conf- the algorithm's first, second and third most likely prediction, favorite_count and retweet_count.

### B. What is/are the main feature(s) of interest in the dataset?

I'm most interested in figuring out:

* Most frequent dog genres predicted by the algorithm
* Most freuqunet dog stages
* Time- Year, Month and hour of tweeting
* Popular dog names
* Correlation coeffiecnt


### 6. Observations and Conclusion
During the vizualization process certain observations have been made and registered after every vizualization. At the end of the analysis the cleaned master dataset has been saved in csv format.


## 7. References

1. [Tidy data by Hadley Wickham, The Journal of Statistical Software, vol. 59, 2014](https://www.jstatsoft.org/article/view/v059i10/v59i10.pdf)

2. Descrition of [Twitter](https://en.wikipedia.org/wiki/Twitter), accesseed on the 29 Jan 2019.

2. Course Content : [Udacity Data Analyst Nanodegree](https://eu.udacity.com/course/data-analyst-nanodegree--nd002)
