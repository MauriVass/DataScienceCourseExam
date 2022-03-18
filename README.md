# Data Science Exam

The objective is to perform a sentiment analysis task, analyzing users' textual reviews, to understand if a comment includes a positive or negative mood.  
In other words, the goal is to build a robust classification model that is able to predict the sentiment contained in a given text.

## Dataset
The dataset for this competition has been specifically scraped from the [tripadvisor.it](https://www.tripadvisor.it/) Italian web site. It contains 41077 textual reviews written in the Italian language.  
The dataset is provided as textual files with multiple lines. Each line is composed of two fields: text and class. The text field contains the review written by the user, while the class field contains a label that can get the following values:  
- **pos**: if the review shows a positive sentiment.
- **neg**: if the review shows a negative sentiment.

The dataset can be downloaded from [here](http://dbdmg.polito.it/wordpress/wp-content/uploads/2020/01/dataset_winter_2020.zip).
## Data exploration
Understand the dataset and the distribution of the data: count the number of elements, check for missing data, mean and standard deviation review length, classes distribution.

## Preprocessing 
Preprocess the data before feeding it to some machine learning algorithm.  
This part consists of the following steps: transform the words in lower case, remove not meaningful words (stop words, too long and too short words), try to balance the classes, calculate the TF-IDF of the words, split the dataset in training and test sets.

## Classification
Apply some machine learning algorithms to train a classifier in order to predict the class of a sentence.  
Many classifiers were used: Support Vector Machine, Naive Bayes, K-Neighbors Classifier, Random Forest Classifier, Decision Tree Classifier, Deep Neural Network, SGD Classifier, Logistic Regression.

## Result
The best model was Linear Support Vector Classifier with a F1 weighted score of 0.9696.

Cloud words of the most common words:  
<img src="https://github.com/MauriVass/DataScienceCourseExam/blob/master/Images/WordCloud.png" width="550" height="280">  
