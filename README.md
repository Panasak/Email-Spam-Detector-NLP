# Email Spam Detector Project: Project Overview
This project uses Natural Langauge Processing and classification to predict whether an email is a spam or not.
* Create a tool that classify email spam to help users identify spam emails
* Engineered features from text to bag of words and tf-idf, in order
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
I looked at the distributions of the data and the value counts for the various categorical variables. Below are a few highlights from the pivot tables.

![alt text](https://github.com/Panasak/Email-Spam-Detector-NLP/blob/main/EDA/pic1.png)
# Model Building
I split the data into train and test sets with a test size of 20%
I used Naive Bayes Classifier and evaluated it using Mean Absolute Error. I chose MAE because it is relatively easy to interpret and outliers aren't particularly bad in for this type of model.
I tried three different models:
* **Multiple Linear Regression** - Baseline for the model
* **Lasso Regression** - Because of the sparse data from the many categorical variables. I thought a normalized regression like lasso would be effective
* **Random Forest** - Again, with the sparsity associated with the data, I thought that this would be a good fit
## Model Performance
The Random Forest model outperformed the other approaches on the test and validation sets
* **Random Forest:** MAE = 4411561.95
* **Linear Regression:** MAE = 441239550501459.25
* **Lasso Regression:** MAE = 6423036.02
