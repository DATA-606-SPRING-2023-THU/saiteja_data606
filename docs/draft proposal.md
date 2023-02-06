## What is your issue of interest (provide sufficient background information)?
- My issue of interest is to classify an SMS into spam or ham (not spam).
- As the usage of mobile phones is increasing, short messages are getting more and more popular.
- Along with that advertisements, spam messages are also getting popular
- The aim of this project is to classify a message into spam or not.
## Why is this issue important to you and/or to others?
- As the sms service is getting cheaper, the usage of sms has been increasing rapidly. Almost all parts of the world are able to use the sms service. This made sms a great medium for spammers to exploit. As days goes y and usage of SMS service increases, the spam messages are also increasing on the network. Many fraudsters are exploiting this service to fool common people.
So a robust solution is required to find these spam messages and filter them. This project aims to build such robust solution.
## What questions do you have in mind and would like to answer?
- Can I use ML techniques to filter the messages? 
- What kind of techniques should I use to create this filter?
- How effective is ML in this case?
## Where do you get the data to analyze and help answer your questions (creditability of source, quality of data, size of data, attributes of data. etc.)?
- I am using a kaggle dataset which contains combination of spam and ham messages
Link - https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset
- It is of 503.66Kilo bytes and contains text messages and their label.
- Data set consists of 5572 rows and 5 columns. Column v1 contains two labels and column v2 contains raw text.
## What will be your unit of analysis (for example, patient, organization, or country)? Roughly how many units (observations) do you expect to analyze?
- The unit of analysis is a single text message and 5169 such units are used.
## What variables/measures do you plan to use in your analysis (variables should be tied to the questions in #3)?
- The text in the message is the input to the analysis. Tfidf vectorization is performed on all words in the dataset to convert the text into numericals. This is important as a computer can only understand numbers but not plaintext.
## What kinds of techniques/models do you plan to use (for example, clustering, NLP, ARIMA, etc.)?
- I will use tfidf vectorization for preprocessing.
- I will use ML models like perceptron, decision tree for the model.
## How do you plan to develop/apply ML and how you evaluate/compare the performance of the models?
- I plan to collect the data first and perform eda. With the results from eda, I am planning to select few models and perform training. Using the trained model, I will perform comparison using various metrics to select final one.
## What outcomes do you intend to achieve (better understanding of problems, tools to help solve problems, predictive analytics with practicle applications, etc)?
- I intend to achieve better understanding on ML algorithms, eda, model comparison, tools used for Machine learning and get familiar with ML model creation process.



