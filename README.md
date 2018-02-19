# Email-Spam-Classification

A classifier that identifies spam emails using Gaussian Naive Bayes


## DataSet description 

The dataset folder consists of emails. If the name of the file contains "spm",then it is a spam message. Otherwise the message is not a spam.
The test dataset are present in test-mails folder
The train dataset are present in train-mails folder

## Feature Extraction

Have used nltk's word_tokenize to build the dictionary out of the words from the emails.
The feature matrix contains the words and the word count. 
The featture matrix is an np array of the form : 
  feature_matrix[doc_id,word_id]   = word_count of the word word_id in the document doc_id
The class matrix is an np array of the form : 
  classes[doc_id] = label of the doc_id

## Model Building

Have used Sklearn library's GaussianNB function to build the model.
Used sklearn metric's accuracy_score to find the accuracy of the classifier. 

