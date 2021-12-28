# Email Spam Detector Project: Project Overview
This project uses Natural Language Processing and Classification to predict whether an email is a spam or not.
* Create a tool that classify email spams to help users identify spam emails
* Engineered features from texts to bag-of-words model and tf-idf, in order
* Used Naive Bayes Classifier to reach a high accuracy
## Code and Resources Used
* **Python Version:** 3.7
* **Packages:** pandas, numpy, matplotlib, seaborn, scikit learn
* **Kaggle Data:** https://www.kaggle.com/datatattle/email-classification-nlp
## About The Data
The data contains the following columns:
* Message Numbers
* Message Bodies
* Labels
## EDA
I looked at the distributions of the data and the value counts for the various categorical variables. Below is the highlight from the pivot tables.

![alt text](https://github.com/Panasak/Email-Spam-Detector-NLP/blob/main/EDA/pic1.png)
# Model Building
I split the data into train and test sets with a test size of 20%. I pre-processed the texts using Count Vectorizer. I then created a function to removed stops words and punctuations from the texts. I turned the texts into bag-of-words model and transformed them into tf-idf, in order.
I used Naive Bayes Classifier and evaluated it using Accuracy. I chose Accuracy because it is relatively easy to interpret.
## Model Performance

* **Naive Bayes Classifier:** Accuracy = 0.92
