# SMS Spam detection
# UMBC Data Science Capstone Project
**Author**: Sai Teja Avadhootha\
**Semester**: Spring2023\
[capstone.pptx](https://github.com/asaitej1/saiteja_data606/blob/main/docs/SMS%20Spam%20detection.pptx)\
[Youtube Link]()\
[capstone.ipynb](https://github.com/asaitej1/saiteja_data606/blob/main/src/sms_spam_detection_(final1).ipynb)

# Introduction
Spam or unsolicited bulk messages are sent out by companies, scammers, and other malicious actors for various purposes. 
Identifying and discarding these frequently taking up space in communication mediums like SMS is necessary.
As the SMS service is getting cheaper, the usage of SMS has been increasing rapidly. Almost all parts of the world are able to use the SMS service. This made SMS a great medium for spammers to exploit. 
As days go by and usage of SMS service increases, the spam messages are also increasing on the network. Many fraudsters are exploiting this service to fool common people.
So a robust solution is required to find these spam messages and filter them. This project aims to build such a robust solution.
Machine Learning algorithms can help in this task by evaluating incoming messages for certain patterns and the likelihood of being spam.
Traditional methods like content-based filtering and headers inspection have inefficiencies. The words used in content can change, therefore ML algorithms like Naive Bayes are used to classify more accurately and quickly.
The objective of this project is to try and experiment with different ML models to perform spam detection and come up with a model that can classify messages into spam and no spam.

# Dataset
The dataset used in this project is a Kaggle dataset which contains a combination of spam and ham messages.
[Dataset Link](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)
It is of 503.66Kilo bytes and contains text messages and their label.

# Unit of analysis
The unit of analysis is a single text message and 5169 such units are used.

# Exploratory Data analysis

