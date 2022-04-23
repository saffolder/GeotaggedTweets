# Geotagged Tweets
### By: Samuel Affolder
---
## Objective
This project was aimed at analyzing the difference in popular words and topics just one week apart in the United States.  Using the Twitter API Crawler I was able to graph the location of Geotagged Tweets in the United States at the two different times that I collected data.  I then put both of those data sets through a word mapping service that shows the prevelance of words in a dataset.

## Reason
The United States media is extremely fast paced and topics come and go in the blink of an eye.  Issues that one day seemed like the end of the world are quickly forgotten.  By having two datasets over a week apart I was able to display the differences in popular terms as noted below.

## Methods
For this project I:
- Registered for an Elevated Twitter Developer Account
- Collected tweets for ten minutes using the Twitter API Crawler in Google Colab
- Mapped the location of the tweets in QGIS
- Created a word art for each dataset

# Outcomes
## Location Mapping
### Tweet Map 01
#### Collected 04/12/2022
![Map of tweet locations](/img/TweetMap01.png)
### Tweet Map 02
#### Collected 04/23/2022
![Map of tweet locations](/img/TweetMap02.png)
## Map Results
When comparing the locations of the two tweet maps the results appear to be very similarly displaced.  The only major difference is the second tweet map has more tweets in the Northeast United States compared to the first tweep map.  This could be due to the fact that the first tweep map contains 3693 tweets while the second tweet map contains 4076 tweets.

---
## Word Mapping
### Word Map 01
![A word map of popular words from the dataset 1](/img/WordMap01.png)
### Word Map 02
![A word map of popular words from the dataset 2](/img/WordMap02.png)
## Word Map Results
While these word maps are interesting to look at and compare, the actual words contained in them are very similar.  These maps only contain the top 200 words in the datasets and thus we can expect that those words would be generally similar.  In order to get a better understanding of topics and trends, a better approach may be to let the crawler run for longer and then compare the words outside of a given threshold, maybe outside of the top 100 most common words.
## Flaws
As noted above, this technique provided insight but could be better if there were not such limiting factors.  For instance, there was a ten minute time limit for the Twitter Crawler to collect tweets and filter them by location.  If the crawler was given even longer to run there would be more data in each dataset.  Another limiting factor was the word maps interpretation of special characters.  The software cannot display emojis or apostrophes and so any word that contains one (ex: can't, won't, it's, they're, etc.) was removed from the dataset.

## Sources
- [Twitter Developer Platform](https://developer.twitter.com/en/docs)
- [Google Colab](https://research.google.com/colaboratory/)
- [QGIS](https://www.qgis.org/en/site/)
- [WordArt](https://wordart.com/)