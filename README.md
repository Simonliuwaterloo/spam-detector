# spam-detector
## Dataset
[Dataset, from Wessel van Lit](https://www.kaggle.com/veleon/ham-and-spam-dataset)
## Algorithm
Use Naive Bayes algorithm, calculate probability of document being spam given document token vector. Classify documents by comparing probability of document being spam with probability of it being ham.
## File structure
[./data/email](https://github.com/Simonliuwaterloo/spam-detector/tree/master/data/email) is the dataset, which has two sub directories, spam and ham, contains spam and ham emails individually  
[spam-detector.ipynb](https://github.com/Simonliuwaterloo/spam-detector/blob/master/spam-detector.ipynb) is my implementation of Naive bayes algorithm classifier  
[spam-detector-sklearn.ipynb](https://github.com/Simonliuwaterloo/spam-detector/blob/master/spam-detector-sklearn.ipynb) is a spam detector implemented with sklearn built-in Naive-bayes algorithm
## Analysis
spam-detector.ipynb has acheived an accuracy of 99.48%, while spam-detector-sklearn.ipynb has an accuracy of only 90.17%. From confusion matrix, we found out that sklearn implementation tend to classify spam as ham.  
However, sklearn implementation is significant (almost 300%) faster than spam-detector.ipynb in terms of training. I am planning to reduce dimension of dictionary with PCA algorithm to reduce training time.
