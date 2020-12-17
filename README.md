# text-data-analysis
Twitter is a modern-day communication phenomenon. For better or worse, it allows people's everyday thoughts to be tweeted and shared geometrically through networks of followers. But many companies and individuals are using tweets in a secondary, introspective way: to track how popular are their brands or products, and to learn what the prevailing opinions are of them. Text analysis can help with that by processing and analyzing the millions of tweets streaming each day, keeping track of the relevant ones.

One useful text analysis technique is sentiment analysis, a form of labeling of tweets based on polarity of opinion: positive, neutral, and negative. While not very accurate, it can give a quick overview of popular opinion and its change over time. Here, you will build a simple tweet sentiment classifier for one specific industry: US airlines.

Data Description: The dataset is called “Twitter US Airline Sentiment”, available as the file Tweets.csv, Preview the documentin the Files section of this Canvas site. (You can also directly read the data using pd.read_csv('https://raw.githubusercontent.com/lkyin/ECS189L/main/Tweets.csv' (Links to an external site.)). It was downloaded from Kaggle as a csv file. Tweets were scraped from Twitter in February 2015 about each major US airline. Contributors then manually classified each tweet as either “positive”, “neutral”, or “negative” and cited the reason for a negative classification as well as a confidence score for the assigned label.

There are 14,640 rows and 15 columns in the data set. The included features are: tweet id, sentiment, sentiment confidence score, negative reason, negative reason confidence, airline, sentiment gold, name, retweet count, tweet text, tweet coordinates, time of tweet, date of tweet, tweet location, and user time zone.


# Part 1: 
As a warmup, consider the sentiment groups of negative, neutral, and positive tweets (airline_sentiment column). For each sentiment group, rank the words used in the text of tweets (tweet text column) by frequency. Eliminate airline names and @-words, as well as stop words and punctuation. 

#Part 2: 
Train a classification model of sentiment as a function of the tweet text. You can use any classification method we studied (no neural nets or others we haven't studied). Use 80% of the data rows for training, and the rest 20% for testing (careful, sample randomly as the tweets are ordered by airline and you want to make sure each airline is represented in both the training and test data). Then, process the text data using best practices in NLP text processing, e.g., eliminate airline names and @-words, any special character words, as well as stop words and punctuation. You may want to lowercase all the words too. If you want to go the extra step, you can use POS-tagging and lemmatization.

# Part 3: 
Rank the different airlines in two ways. First, in terms of the fraction of positive tweets. And second, in terms of the fraction of negative tweets.
