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

# SVM
Support vector machine is a classification algorithm that uses a hyperlane to split between data points of different classes in such a way that it maximizes the margin between them.

# Decision tree
A decision tree is a type of machine-learning algorithm used for both classification and regression tasks. It involves creating a tree-like model of decisions and their possible consequences. The model is built by recursively splitting the dataset into smaller subsets, based on the value of one of the input features, in a way that maximizes the information gain or minimizes the impurity of the resulting subsets.
At each internal node of the tree, a decision is made based on the value of the input feature and the tree branches out to the next node until a leaf node is reached, which represents the prediction or classification of the input. Decision trees can handle both categorical and continuous input variables and are easy to interpret and visualize, making them a popular choice for tasks such as predictive modeling, data mining, and pattern recognition.

# Multi-layer perceptron
Multilayer perceptrons (MLPs) are a type of artificial neural network.
They consist of multiple layers of interconnected neurons.
Each neuron uses an activation function to introduce nonlinearity into the network.
MLPs are trained using an optimization algorithm such as backpropagation.
They are commonly used for supervised learning tasks such as classification and regression.

# Random forest
Random Forest is an ensemble learning algorithm.
It combines multiple decision trees to improve predictive accuracy and reduce overfitting.
Each tree is trained on a randomly selected subset of the input features and data samples.
The final prediction is obtained by aggregating the predictions of all the trees.
Random Forest is widely used for classification and regression tasks in various domains.

# AdaBoost
AdaBoost (Adaptive Boosting) is a type of ensemble learning algorithm.
It combines multiple weak classifiers to form a strong classifier.
During training, each weak classifier focuses on the misclassified samples of the previous classifier.
The final prediction is obtained by aggregating the predictions of all the weak classifiers. AdaBoost is widely used for classification tasks in various domains.

# Results
## Confusion matrices
### SVM
<img width="500" alt="image" src="https://github.com/asaitej1/saiteja_data606/blob/main/Images/SVM.png">

### Decision tree
<img width="500" alt="image" src="https://github.com/asaitej1/saiteja_data606/blob/main/Images/Decisiontree.png">

### MLP Classifier
<img width="500" alt="image" src="https://github.com/asaitej1/saiteja_data606/blob/main/Images/MLP.png">

### Random forest
<img width="500" alt="image" src="https://github.com/asaitej1/saiteja_data606/blob/main/Images/Decisiontree.png">

### AdaBoost
<img width="500" alt="image" src="https://github.com/asaitej1/saiteja_data606/blob/main/Images/AdaBoost.png">

- In SMS spam detection, false positives are the most important concern. Moving spam to non-spam may not cause big trouble but moving a non-spam to spam may cause the user to miss out on important information.
So, we chose Random forest which had false positives as our final model.

# Conclusion
Using Machine Learning, spam messages from legitimate messages can be identified and classified accurately. The accuracy of the model can be further improved by fine-tuning the parameters. Moreover, this solution could be deployed in an industrial setting as it does not require any human intervention to continuously detect spam messages in real time.
