# Sentiment_Analysis
The aim of this project is to build and critically analyze some ML methods to predict star rating (1,3,5) for reviews on restaurants in Yelp.

The raw review text of the datasets were collected from Yelp. This project mainly used the representations, which processed by CountVectorizer and doc2vector methods, to build and develop our classifiers. CountVectorizer is an encoding method, which represent the count vectors as a sparse matrix. While the doc2vector focus on creating a numeric representation of words in high dimensions. 
   
Furthermore, the training dataset provided was randomly splitting into training and validation set so that we can train and adjust our models before predict the labels of unseen testing dataset.

This project choose two popular models in text classification, which is Multinomial Naive Bayes(MNB) classifier and linearSVC. MNB classification is often used as a baseline solution in text classification due to its high efficiency.(3) It is a specific variants of Naive Bayes where assumes that all the pairs(P(Feature i|Class)) of data follows multinomial distribution. For LinearSVC, it is a hyperplane-based classier for binary classification problems. In section3.2, the analysis of LinearSVC with sparse matrix will focus on the improvement of accuracy by selecting features or tuning parameters.


# Conclusion
In this project, we experimented with 3 models including MNB classification, LinearSVC and bagging ensemble model. Examining the analysis above, we found that linear classifiers tend to work well on sparse datasets since the sparse matrix is very likely to be linearly separable and SVM is good at handling high dimensional datasets. By filtering features and tuning parameter, the performance of LinearSVM only has a slightly increase, which shows that the problem is not very complexity.
