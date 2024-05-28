# Spam Tweet Research
Developed a network analysis prediction of highest spam indicators on Twitter using 10,000 tweets from Nsc.org, a leading research lab on cybersecurity. Trained and tested data using Naive Bayes, Random Forest, and KNN. Utilized Machine Learning toolkits (TensorFlow, keras) and Python.

# Intro
Social networking platform Twitter is a prominent victim of spam. Spam can drown out important news, leading to misinformation, and is often the cause of malware and scams. My data was collected from Nsc.org, a research lab on cybersecurity. Their database contained 6 million tweets. 10,000 were randomly selected from the ‘continuous’ folder, meaning the tweets were sent in a continuous time frame. This was to optimize the running algorithms and for demonstration purposes.

The tweet data I sourced contained a very extensive feature set. It included: account age, number of followers, number of followed, number of favorites on the tweet, number of lists added by the user, number of hashtags in the tweet, number of tweets sent by the user, number of characters in the tweet, etc.

Algorithms used: Random Forest, Naive Bayes, K Nearest Neighbor, and a self-implemented K nearest neighbor graph.

# Results
The most accurate algorithmic classifier for predicting spam was Random forest when n is set to 100, with an accuracy of .954. The least accurate algorithmic classifier was Naive Bayes, with an accuracy of .566. The most influential tweet features that indicate spam were 1) numbers of characters in a tweet and 2) numbers of hashtags in a tweet. 

My self-implemented KNN graph seemed most realistic with k set to 3. As I increased K, I found that the graph began to prefer the prediction of non-spammers. The most reasonable epochs for training would be about 20 due to the fact that accuracy and loss level out around that value. My self-implemented KNN graph had the highest prediction accuracy, eventually reaching 100% as seen by keras.



