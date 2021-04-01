# Sentiment-Analysis

Sentiment analysis is one of the Natural Language Processing techniques for finding out the opinion or sentiment of the user regarding a product or movie or hotel or any real 
world thing that can have an opinion.Sentiment analysis can be highly useful in several cases. One such example is marketing techniques.It can also help users to decide when 
going for movies,online shopping,hotels and endless similar situations.Social media platforms like Twitter, Facebook,YouTube, Reddit generate huge amounts of big data that 
can be mined in various ways to understand trends,public sentiments and opinions.Sentiments can be analyzed and classified either by machine learning techniques or by 
Lexiconbased techniques. With the help of sentiment analysis companies can use huge chunk of information that is shared online daily to track public likes and dislikes.

Implementation of Basic Naïve Bayes Algorithm for the sentiment analysis of the positive and negative reviews of the many hotels using train set which consistes of 
positive and negative hotel reviews. Naive Bayes is a classification algorithm that is based on Bayes theorem with an assumption of independence among predictors that is 
It assumes that the presence of a particular feature in a class is unrelated to the presence of any other feature.
                                                             Posterior=(prior * likelihood)/evidence

As a first step, Regular Expressions are used to clean up the data, that is, to eliminate the punctuation marks - !,?,-,. Etc and to eliminate frequently repeated words called 
Stop Words, like ‘the’,’a’ etc., the Stop Word dictionary from nltk package was used. Laplace Smoothing is done to avoid zero probabilities appearing for likelihood.
Likelihood probability for each word is calculated as a ratio of frequency of each word to the sum of frequency of all other words in the class and size of the vocabulary for 
that class. For calculating the Prior P(c), the fraction of number of reviews in each class to the sum of number of reviews in both the classes is considered. 
To avoid underflow, all the probabilities are calculated with log to the base 10. And unknown words are ignored. Finally for test set, the probability for each review 
is calculated for each class and whichever class has the highest proabability value, the review is assigned that particular class. The class being POS and NEG here 
representing Positive and Negative Reviews.

The given training set is divided in the ratio of 80:20 for training and testing the data. The accuracy achieved was around 88% using the Basic Naives Approach.
My second approach is using naïve bayes library of textblob for higher accuracy. With this library, the accuracy achieved was around 90%. 


