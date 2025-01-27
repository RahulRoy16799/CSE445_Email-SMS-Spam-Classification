Users can send and receive messages quickly and cheaply over the internet by using Email. Although email is a useful tool for
exchanging information, occasionally spam is sent in mass to a large number of recipients. The idea of spam is broad because it might include
chain letters, unwelcome adverts, and other things. Spam causes wastage of resources and it is very annoying problem which is being faced by
almost everyone having an email account. So, filtering spam email before sending it to user’s inboxes is a crucial and difficult undertaking.
With this proposed model the specified message/mail can be stated as spam or notspam using Bayes theorem, Naïve Bayes Classifier and
others.
We know, with the growing use of email communication, Email spam has become a significant challenge in recent years. Spam
emails not only consume valuable time and resources but also pose a security threat as they may contain malicious content or links. The
proposed system has practical applications in improving Email/SMS filtering for individuals and organizations by reducing the number of
unwanted or malicious emails/SMS that reach their inboxes. This project has the potential to contribute to the field of email security and spam
filtering by providing a more effective and efficient solution. In this project, we have taken e-mail Spam-Ham dataset from Kaggle– “E-mail
Spam Collection Dataset”. The project will involve several stages, including data collection and text preprocessing, model building,
evaluation and improvement. For further improvement, we could build a website by creating a pipeline and deploy. We will explore
various machine learning algorithms such as Naive Bayes, Decision Trees, Logistic Regression, Extra Trees Classifier etc.
The proposed system has practical applications in improving email filtering for individuals and organizations. By reducing the number of
unwanted or malicious emails, the proposed system will help individuals and organizations to save time, increase productivity and minimize
security risks.

As a specific output we want to predict whether an e-mail as a Spam or Ham (i.e. not Spam) one. From the dataset we had 5572 rows, but after
the data cleaning process (i.e. Removing 415 duplicate values, by keeping the original values) we got 5157 rows. The dataset is saved in the
‘kaggle’ website and can be accessed via link mentioned above. The dataset was last updated 2yrs ago. Changes/biases was normalized in the
data cleaning process. The most relevant factors for predicting our specific output was Accuracy, Precision, Recall and Confusion Matrix. But, we are mostly
concerned about the Precision than the accuracy, since our dataset is large and in thiscase, Precision is particularly useful when the
cost of false positives is high, such as in medical diagnoses or spam email classification. We are hoping to use 10 fold cross validation
where the algorithm is then trained on nine of the folds and the remaining fold is used for testing. This process is repeated ten times, each
time using a different fold for testing, and the results are averaged to give an overall performance metric. We did 90-10 train test
split. For the simple benchmark to compare the result against, is to predict/ asses the result by comparing the value of Accuracy, Precision and
the Confusion Matrix. Again, another benchmark of comparison is number of characters, words and sentences and even the mean of these
three, are usually greater in value for the Spam messages than the Ham messages. The minimum level of accuracy we expect is 86%. 
To clarify our vision, we will create a pipeline from the codes and convert it into a website, where we expect to have a box (text field) in a window where we will provide the
input texts for the testing sets and then by pressing the predict button it will give the result accordingly as spam or not spam. Each testing
data will have to perform the following three steps in the pipeline before showing the result in the website though ‘Streamlit’ (an open-source
app framework for Machine Learning):
a) Text preprocessing (Lower casing, Tokenization, Removal of special words, stops words and punctuations, Stemming)
b) Vectorization(Converting textual data into numerical vectors
c) Application of different algorithms

The Voting Classier is working the best, since it’s giving the highest accuracy with 100% precision that is, no false positives are there. So,
we will hopefully proceed with this algorithm.
