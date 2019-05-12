# NLP-Naive-Bayes-based-spam-detection
This project builds a Naive Bayes classifier to predict whether a text message is spam or ham.

# The data set
The data set comprises of a .csv file which contains several text messages each of which has been labelled as either spam or ham.

# Data pre-processing
A custom preprocessing function is written which comprises of the following steps:
1) Change the input document/string to lowercase
2) Tokenize the document/string into words
3) Remove the stop words
4) Stem or Lemmatize the words obtained through steps 1 to 3 above

This fucntion returns a list of preprocessed words.

# Feature creation and data preparation
The features for each document in the data set are the unique words present in all the documents of the data set.
A custom function to extract all the unique words from the data set is built. The dataset is subsequently divided into training and test data in the ratio of 80:20. The features as described above are extracted from the training and test data sets.

# Model building
NLTK's NaiveBayesClassifier() class is used to train a Naive Bayes model on the training data set.

# Model evaluation
The Naive Bayes classifier gives an accuracy of 98.3%.
