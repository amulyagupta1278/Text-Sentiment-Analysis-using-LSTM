# Text-Sentiment-Analysis-using-CNN-LSTM-and-LSTM-CNN

With the recent advances in neural networks and the hardware technology needed to support the computations they demand, the field of Information Retrieval - which has traditionally been associated with search engines and index construction - is witnessing an upward trend in the research toward Emotion AI, where the term  Emotion AI refers to the subset of artificial intelligence that measures, understands, simulates, and reacts to human emotions.

Sentiment Analysis, sometimes also referred to as opinion mining, finds itself at the junction of Emotion AI and traditional IR, where the efficient index construction and text vectorization techniques meet the more recent neural networks - including, the increasingly popular convolutional neural networks and RNN-based sequence models - “to systematically identify, extract, quantify, and study affective states and subjective information” from the user input.

Although a pipeline for sentiment analysis may benefit from inclusion of visual - for instance, a photograph of the tweeter’s face, showcasing their emotions at the time of posting the tweet - and audio - variations in amplitude and frequency of the speaker - cues, we shall focus solely on the more traditional view of sentiment analysis where it is applied on textual data. Particularly, we shall take up the ideas in (Haque et al) to build neural network based classifiers for binary sentiment analysis for movie reviews, designating them as positive or negative reviews. We will explore the three different neural network architectures - LSTM, CNN, and LSTM-CNN - used for the task and benchmark them against each other and classifiers used in related literature.

## Problem Statement

The general classification problem in IR is formulated as follows: given a set of training documents, D, and the corresponding labels, cD, use a supervised learning method, , to learn a classifier, : X  C - where X is the document space and C = {c1, c2, ..., cN} is the set of all classes involved - that maps a document d X  to its corresponding class c [4].

In our version of the sentiment analysis problem, we define X to be the set of all IMDb movie reviews, D to be our training partition of the dataset, and C = {pos, neg} for positive and negative reviews. Furthermore, we use three supervised learning methods 1 LSTM, 2 CNN, and 3 LSTM-CNN to learn three instances of the classifiers 1= 1(D), 2 = 2(D), 3 = 3(D) to classify any new - or test - movie reviews as positive and negative. Thus, the sentiment analysis task has been posed as a binary classification problem.
