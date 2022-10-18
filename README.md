# NaiveBayesClassifier / Parody on Machine Learning

*Program to predict whether the message is spam or not*

## To see all explanations and all the work open file "Lab1_Naive_Bayes_Classifier_Templatee.html"


 
#### Some results ran on the test data:




<img width="1194" alt="Screenshot 2022-10-18 at 23 24 24" src="https://user-images.githubusercontent.com/92575094/196536468-b249c4ae-4edd-4c16-87ef-7311c4cc566a.png">




<img width="1070" alt="Screenshot 2022-10-18 at 23 24 42" src="https://user-images.githubusercontent.com/92575094/196536526-b22a43fc-a221-43c8-acd7-ffdcd90ed176.png">



<img width="988" alt="Screenshot 2022-10-18 at 23 25 04" src="https://user-images.githubusercontent.com/92575094/196536591-b1e97b72-6a0a-419a-b1fd-16c649c38af0.png">


- The implemented method is Naive Bayes Classifier. We used it to predict the Category of a message. Choosing the probable category means calculating the probability of message belonging to each category and then picking the highest one. Since it is very unlikely for the message to repeat in train data, we divide the message into clean words (lowercase + no punctuation marks). Then probability for sentence = product of probabilities of each word. The bag-of-words helps quickly find matches in the training data.

- The method doesn't process the meaning of a sentence, and just counts words.  The non-spam message might include words that often appear in spam. Then, the Classifier will mark it a 'spam'. It works vice versa too. To improve this method, words can be stored as phrases. Despite that, the method is easy to understand and quite effective to filter spam messages. As stats show, only 6 out 1061 non-spam were wrongly identified as spam.
