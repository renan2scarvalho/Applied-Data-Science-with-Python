# Content:
- Understand how text is handled in Python;
- Write code that groups documents by topic;
- Apply basic natural language processing methods;
- Describe the nltk framework for manipulating text.

## Work: Twitter Sentiment Analysis

The work consisted in performing a sentiment analysis with collected tweets with the topic *covid*. 
The pipline consisted in connecting to NoSQL MongoDB, collect tweets with Tweepy API, and analyze the tweets.
Here the tools for classification were:

1. Naïve Bayes
2. Support Vector Machines
3. TextBlob
4. VADER

To help understand better the tools, a beforehand hand-on classified dataset was used to compare results of "unlabeled" algorithms (TextBlob and VADER), and also used as a training set for the word vector algorithms NB and SVM.
