# Classification-of-Political-Tweets-and-Detection-of-Bots
Machine learning techniques and feature extraction will be employed for the classification of political tweets and identification of bots in the project.

This ML and feature extraction-based project aims to analyze tweets and user metadata to identify whether a tweet is political and if a user is a bot. The project is divided into three parts: feature extraction, tweet classification, and bot classification. The goal is to provide probability scores between 0 and 1 for users  **(isBot)** or tweets **(isPolitical)** and minimize the mean square error between predicted values and actual labels. The project has three steps, each aimed at optimizing the predictors and reducing ***MSE values***.

The feature extraction process involves major analyses described in the extraWorks file, while the tweet_experiment file contains the main implementation of the project with detailed explanations. All relevant data files are also available.

### For data,
- the given dataset was used for model training. 
- The dataset was merged with corresponding JSON files to obtain the desired features for training.
-  All tweets in the user_tweets JSON file were analyzed to create political entity lists for detection.

## Features that obtained from Tweets,
- **Check for Political Entity in Text**
The project checks for the presence of political entities such as RTErdogan and vekilince in tweets. These entities are often indicative of political content.

- **Number of Total Interactions**
The project counts the total number of interactions a tweet has received, including the number of tweets and retweets. This information can be useful in identifying popular or influential tweets.

- **Source Detection**
The project also identifies the program used for tweeting and which API was used to produce the tweet. This information can be helpful in identifying suspicious activity that may indicate the presence of a bot.

- **Check if Retweet**
The project checks whether a tweet is a retweet or not. Retweets may contain political content and can be used to spread propaganda or disinformation.

- **Get Tweet Text**
The project retrieves the text of a tweet. This information can be used for sentiment analysis and to determine the presence of political content.

- **Get Number of Retweets and Favorites**
The project also counts the number of retweets and favorites a tweet has received. This information can be useful in identifying popular or influential tweets.

## Features that obtained from users,
- **Get User Info Metadata**
The project retrieves user metadata such as name, location, and profile description. This information can be used to identify the interests and affiliations of the user.

- **Get Followers/(Followers+Friends) Ratio**
The project calculates the ratio of followers to total connections (followers + friends) for a user. This information can be used to identify the popularity and influence of the user.

- **Get Creation Time**
The project retrieves the creation time of a user account and checks whether the account was created consecutively or not. This information can be useful in identifying bots that create multiple accounts in a short amount of time.

- **Get Description Length**
The project checks the length of a user's profile description. This information can be used to identify the interests and affiliations of the user.

- **Check Ratio of Retweets to All Tweets**
The project checks the ratio of retweets to all tweets for a user. This information can be used to identify users who primarily retweet content rather than creating original tweets.

- **Check Median Number of Favorites**
The project checks the median number of favorites a user's tweets receive. This information can be useful in identifying popular or influential users.


## For the models:

- **Decision Tree Classifier:** This model uses a tree-like graph to classify data based on features such as political entities, interactions, and source detection.
- **XGBOOST:** This is a gradient boosting model that is used to classify tweets and users based on their features.
- **Logistic Regression:** This model is used for binary classification tasks and is used to classify tweets and users as political or non-political and bot or non-bot.
- **Naive Bayes:** This probabilistic model is used to classify tweets and users as political or non-political and bot or non-bot.
- **Neural Network:** This model is inspired by the structure and function of the human brain and is used to classify tweets and users based on their features.

All models use a combination of tweet and user features, including the presence of political entities, number of interactions, source detection, followers ratio, creation time, and description length to accurately detect Twitter bots and classify tweets as political or non-political.



