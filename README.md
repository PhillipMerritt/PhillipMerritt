# Phillip Merritt Portfolio

## [Subreddit Sentiment Tracker](https://github.com/PhillipMerritt/SubredditSentimentTracker)
* Allows users to analyze the changes in sentiment over time in online communities

  e.g. A developer that wants to see an overview of the reaction to recently released update could generate a chart of sentiment over the days before and after the update.
* Full stack webapp created using Vue.JS and Flask
* Comments from the specified subreddit and time range are pulled from the pushshift API
* Those comments are sent to the backend where sentiment analysis is performed from a variety of NLP packages
* The average sentiment for discrete time segments is sent back to the frontend where a chart of the data is generated

