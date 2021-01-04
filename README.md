
# **SpamClassifier**
## **Predicting Whether a Message is Spam or not.**

<img src="https://github.com/manthanpatel98/SpamClassifier/blob/master/README-Resources/SpamClassification.jpg" width=600>


---
### Web APP on Heroku

<img src="https://github.com/manthanpatel98/SpamClassifier/blob/master/README-Resources/Spam.gif" width="600">

### **[The Project on Heroku](https://spamclassifiersms.herokuapp.com/)**

---
## **Understanding The Project**

### **The Dataset**
***
#### **Initial Dataset**
![Dataset](https://github.com/manthanpatel98/SpamClassifier/blob/master/README-Resources/Screenshot%20(100).png)
#### **Converted into Structured Dataset**
![Dataset](https://github.com/manthanpatel98/SpamClassifier/blob/master/README-Resources/Screenshot%20(101).png)

---
## **Overview**
* Message and its final output is separated by Tab space.
* From the Dataset, we have to predict the **label** column: 
* **PortStemmer** method has been used for **Stemming**.
* I have applied many different algorithms **RandomForestClassifier**, **MultinomialNB**, **SVM** and **KNN**.
---
## **Details**
* Here, Initially in our data, Message and its final output is separated by Tab space so i have separated them by Tab and created 2 columns **"label"** and **"message"**. 
* Then, line by line after converting each line in lower case, **PortStemmer** has been used and have created matrix for words that are not in **stopwords**.
* This project has around **5572** Messages, so for **CountVectorizer** in Bag of Words **max_features=2500** gave the best results.
* In this Project, I have tried **RandomForestClassifier**, **MultinomialNB**, **SVM** and **KNN**. 
* To understand detailed Project approach, check my [**SpamClassifier.ipynb**](https://github.com/manthanpatel98/SpamClassifier/blob/master/SpamClassifier/SpamClassifier.ipynb) or [**Spamclassifier.py**](https://github.com/manthanpatel98/SpamClassifier/blob/master/SpamClassifier/Spamclassifier.py)

***
### **Applied Algorithms & Their Accuracy**
***
| Algorithm | Accuracy |
| ---    | ---    |
| Random Forest | 98.20% |
| MultinomialNB | 98.57% |
| SVM | 85.65% |
| KNN | 98.08% |

* After Checking Accuracy for these Four Algorithms, I decided to use **MultinomialNB** in **Web App**.
* For NLP Projects MultinomialNB works generally better.
