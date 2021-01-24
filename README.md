# Phillip Merritt Portfolio

## [Subreddit Sentiment Tracker](https://github.com/PhillipMerritt/SubredditSentimentTracker)
* Allows users to analyze the changes in sentiment over time in online communities

  e.g. A developer that wants to see an overview of the reaction to recently released update could generate a chart of sentiment over the days before and after the update.
* Full stack webapp created using Vue.JS and Flask
* Comments from the specified subreddit and time range are pulled from the pushshift API
* Those comments are sent to the backend where sentiment analysis is performed from a variety of NLP packages
* The average sentiment for discrete time segments is sent back to the frontend where a chart of the data is generated

  ![](https://github.com/PhillipMerritt/PhillipMerritt/blob/main/images/subredditsentimentdemo.gif)
  

## [nnViz](https://github.com/PhillipMerritt/nn_viz)
* Unity program that allows users to create a 3D vizualization of the internal state of an uploaded neural network and sample inputs
* Written in C# and python
* The python hook takes the user uploaded tensorflow model and retrieves the internal state of each layer for each input then encodes this data in JSON
* The convolutional layer activations and a sampling of the dense layer connections are read from the JSON encoding and rendered in 3D.

  ![](https://github.com/PhillipMerritt/PhillipMerritt/blob/main/images/nnViz_demo_edited.gif)

## [AlphaDomino](https://github.com/PhillipMerritt/Alpha_Domino)
* Working implementation of the AlphaZero reinforcement learning algorithm in python
* Uses a Information Set Monte Carlo Tree Search algorithm which is a modified MCTS that enables the usage of tree searches for games with hidden information like dominoes
* Game state is encoded in binary vectors which is passed to the value prediction Keras CNN to simulate a MCTS rollout
* Self-play, training, and evaluation are all performed in parallel
* Agents trained in Texas 42 won against the baseline 95% of the time and performed at a level sufficient for our research at the time
