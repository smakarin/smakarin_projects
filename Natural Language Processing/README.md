
## Text Sentiment Analysis
### Toolkit
Libraries nltk and spacy.  
Text preprocessing, lemmatization, and vectorization.  
Sklearn models and BERT.  
### Introduction
An online store is launching a new service where users can edit and augment product descriptions.  
We need to build a classification model for comments into positive and negative ones.  
We have a dataset with toxicity labels available.  

### Goal
Train a model to classify comments into positive and negative.

### Project Structure 

1. Studying the data and preparing it for training:
   * Conducting lemmatization;
   * Cleaning up unnecessary symbols;
   * Vectorization of comments using the tf_idf method;
   * Training traditional prediction models;
2. Using BERT;
3. Analyzing the results.

### General Conclusion

In this work, we trained a model to classify comments into positive and negative categories. The logistic regression model, trained on vectorized and balanced data, displayed the best performance in terms of quality and speed - with an f1 score of 0.76 and a wall time of 6.6 seconds.  

The use of BERT yielded the following results:  
With a sample of 200 comments, BERT, in combination with logistic regression, achieved an f1 score of 0.67 with a run time of about 4 minutes. On a sample of 2000 comments, the result was 0.72, with a runtime of 35 minutes. We can hypothesize that the result on the full dataset would be approximately 0.8, but the training would take a significant amount of time in this case.  
