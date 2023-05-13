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
The dataset used in this project is a Kaggle dataset which contains a combination of spam and ham messages.\
[Dataset Link](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)\
It is of 503.66Kilo bytes and contains text messages and their label.

# Unit of analysis
The unit of analysis is a single text message and 5169 such units are used.

# Exploratory Data analysis

<img width="500" alt="image" src="https://github.com/asaitej1/saiteja_data606/blob/main/Images/Image1.png">
In the above graph, we can see the distribution of ham and spam messages in the dataset. We can see that the data is a bit imbalance and ham messages are present more in number than ham messages.

<img width="500" alt="image" src="https://github.com/asaitej1/saiteja_data606/blob/main/Images/Image2.png">
In the above figure, we can see that most of the sentences are less than 200 characters or 30 words in size. So, we can perform classification using simple ML models like SVM etc.

<img width="500" alt="image" src="https://github.com/asaitej1/saiteja_data606/blob/main/Images/Mostusedwords.png">

# Preprocessing
The preprocessing method used in this project is TFIDF vectorization. 
TF-IDF stands for Term Frequency-Inverse Document Frequency 
It is a technique used to transform text data into a numerical representation that can be processed by machine learning algorithms. 
It assigns weights to each word based on how frequently it occurred in a document and in the entire corpus.
This weight can be used to perform numerical comparisons between words

# Models trained
- Support vector machine
- Decision tree
- Multi layer perceptron
- Random forest
- Ada Boost

