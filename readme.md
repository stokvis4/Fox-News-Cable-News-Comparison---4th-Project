# Project Fletcher

Metis - NYC 2018 DS 14 - Project Fletcher.

Completed: March 1, 2018



[Blog Post](https://stokvis4.github.io/Third-Blog/)

[Repository](https://github.com/stokvis4/projectFletcherGit)


## Overview:


# Comparing Cable News Hosts

### Goal:
The goal of this notebook is to explore the commentary of the hosts for each of the three main cable news networks using unsupervised learning methods.

### Shows
Fox News:
   * Tucker Carlson Tonight
   * Hannity
   
CNN:
   * Erin Burnett Outfront
   * Anderson Cooper 360
    
MSNBC:
   * All In with Chris Hayes
   * The Rachel Maddow Show

### Data Sources:
I used a combination of Selenium and BeautifulSoup to scrape the transcripts. For CNN and MSNBC, I pulled from their respective websites. For Fox News, I used Fox News's website to pull Hannity and used Archive.org's transcipts to pull Tucker Carlson Tonight. 



### Date Range:
I pulled data from the beginning of 2016 but the majority of my analysis comes from the beginning of 2017 onward.


### Conclusions:
Fox News's success is due to many factors. Fox News exploits behavioral economic biases to beat the competition consistently. Three of the noticeable ones that I explore in this notebook are the following:


* **Emotion** - Fox News hosts make a noticeably higher amount of statements that are emotional. Using the VADER Sentiment tool, I plotted positive and negative statements by each host for each transcript. Fox News consistently appears to have a higher level of negative statements compared to the other networks. By stoking negative emotions in their audiences, they exploit the negativity bias of their audiences.


* **Catchphrases** -  Just as Trump created memorable catchphrases for his campaign rivals (we all remember "Low Energy Jeb" and "Crooked Hillary"), Fox News hosts have memorable catchphrases that their audiences can grab onto and remember. Using ngram analysis, I was able to derive common phrases for each host. While MSNBC and CNN hosts refer to newspapers (like "Wall Street Journal" and "New York Times") and generic statements (like "We'll be right back"), Fox News hosts have memorable lines. For Hannity, he coined the phrase "Destroy Trump media" to refer mainstream media sources. For Tucker Carlson, the combination of the phrase "the show that is the sworn enemy of lying, pomposity, smugness, and groupthink" appeared multiple times. 


* **Create an Enemy** -  Fox News hosts have successfully created multiple enemies that allow them to frame an issue they bring up. Using NMF  topic modeling, I was able to compare the topics that the hosts focused on. For Hannity, he has created an enemy by tying Hillary Clinton to multiple issues, including the Steele Dossier, Special Counsel invesitigation, and the most surprising, the #MeToo movement. Additionally, he's created an enemy in the media which is the topic of one grouping and mentioned in another. By associating Hillary Clinton with multiple topics, he is able to frame issues in his audience's heads by exploiting the availability heuristic.


