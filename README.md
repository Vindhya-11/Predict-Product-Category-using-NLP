## Predict-Product-Category-using-NLP
Goal is to predict the product category.
In this project, I have tried to predict the category of the products based on the given attributes, among them  Description is the main feature.
I have only considered Only five category from the total set.
Dataset link: https://docs.google.com/spreadsheets/d/1pLv0fNE4WHokpJHUIs-FTVnmI9STgog05e658qEON0I/edit?usp=sharing
## Data Preprocessing
The pre-processing for text data is quite different from the normal dataset. The text data first needs to be converted to a numeric representation before ML algorithms are applied to it. The methods which achieve this goal are called text vectorisation methods. The most popular ones are Bag of Words, TF-IDF and Word2Vec. In most cases, they result in what is called a Term-Document matrix (TDM). I have used TF-IDF in this model
The text vectorisation methods are coupled with pre-processing steps like n-grams, removing stop-words, stemming etc. n-grams takes blocks of 2 consecutive words or 3 consecutive words, in-addition to single words, while creating a TDM. Removing the stop words excludes the punctuation marks and other inconsequential words like articles (a, an, the) prepositions and conjunctions (about, among, anyhow etc.) from the TDM. Stemming prunes a word to its root. Plural becomes singular, different tense variants reduce to their simple present form.
## Data Visualisaton
In order to understand the composition of the dataset, I have looked into univariate distributions (probability distribution of just one variable) by showing labels frequency with a bar plot.


![image](https://user-images.githubusercontent.com/54469298/114268632-b4a04c80-9a1f-11eb-8bbf-826b9d867792.png)
## Algorithm and Improving Accuracy:
Once the text data has been converted to a numeric representation, it is ready to apply classification models. The most popular algorithms which are used for text classification are Multinomial Naïve Bayes and Support Vector Machines (SVM).
I have used Naïve Bayes Algorithm in this model. It is a probability based classification method. It calculates the conditional probability for a block of words (product title) to belong to a particular class (product category). A product title is assigned to the product category for which the conditional probability is the highest
## Output
Eg: Input the 'Mobile' string to test and we will get its product category i,e Mobile & Accessories.
![image](https://user-images.githubusercontent.com/54469298/114268582-6b4ffd00-9a1f-11eb-9332-5e6f33ef3914.png)


