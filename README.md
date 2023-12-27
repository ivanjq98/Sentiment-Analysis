# Sentiment-Analysis
Sentiment analysis (a.k.a opinion mining) is the use of natural language processing (NLP) to determine
the polarity (i.e., positive, negative and neutral) of a given piece of text. You are required to build a
learning-based classifier to classify the sentiments of product reviews. The whole process involves the
following steps:
1. Reading in data: In this project, you will be using product review data [1]. You will need to
load the data from the provided json files. There are two csv files, namely training set
(“train.json”) and testing set (“test.json”), each contains examples in the dataset splits. The
attributes of the data are as follows:
a. reviews – the user review of the product (in raw text)
b. sentiments – the ground truth sentiment of the review, where 0 represents negative
and 1 represents positive.

2. Data processing: You will need to convert the raw data into appropriate feature format such
as via bag-of-words models (e.g., TF-IDF), pretrained word embeddings model [2,3] or
pretrained language models [4]. The procedures in this step may vary according to the feature
format selected. You may refer to the “tfidf_features_example.ipynb” for an example on how
to convert the review from raw text to TF-IDF features.
3. Model Selection: You are to design and develop a classification model to classify the
sentiments of product reviews. You are encouraged to use neural networks for this task. For
example, you can treat the review as a sequence and embed them using recurrent neural
network (RNN) or pretrained language model such as BERT [4], then pass the embeddings to
a classifier layer.

4. Training: You will need to try different model parameters to obtain good classification results,
e.g., feature dimension, weights, initialization, and learning rate. In the training stage, your
algorithm should take only the inputs from the training set and predict their corresponding
labels.
5. Prediction: By setting up the correct learning algorithm, you can classify the sentiment of the
reviews in the test set.
