### This is just for me to review my own work on pulling Reddit comments

# Natural Language Processing & Webscraping project
This repository houses the information and working files used to pull, process, and analyze data for DSI project 3.

The task was to pull text data from a website (reddit) and use a combination of Natural Language Processing (NLP) and classification techniques to predict outcomes. Specifically the primary task is to predict "subreddits" and the secondary goal it to predict whether a given block of text is a Post or a Comment.

The repository is organized as follows:

* **datasets**
  * There are four parent .csv files holding "Posts" and "Comments" data for "Astrophysics" and QuantumComputing"
  * Each parent is paired with an EDA file which contains similar data but cleaned out
* **images**
  * Two .png files showing the frequency of user posts over time for each of "Astrophysics" and "QuantumComputing"
* **misc**
  * Several code-along notebooks whose code was reproduced in whole or in part in several main notebooks in the "notebooks" directory
  * They are included for completeness' sake but not necessary to the analysis otherwise
* **notebooks**
  * Pulling data
    * Making use of the PushShift API to pull reddit posts and comments, and stores them as .csv files in datasets
  * EDA
    * Initial exploration and cleaning of the datasets, plus useful statistics found along the way
  * The model notebooks are categorized as AdaBoost, LogisticRegression, RandomForest
  * Each model category is further branched by four datasets:
    * reddit Posts only
    * reddit Comments only
    * reddit Posts and Comments (combo)
    * reddit Posts and Comments, but to predict post/comm status rather than subreddit category
