# Goal:
To predict whether news provided is real or fake

# DATASET:
https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification

# Description:
(WELFake) is a dataset of 72,134 news articles with 35,028 real and 37,106 fake news. For this, authors merged four popular news datasets (i.e. Kaggle, McIntire, Reuters, BuzzFeed Political) to prevent over-fitting of classifiers and to provide more text data for better ML training.

Dataset contains four columns: Serial number (starting from 0); Title (about the text news heading); Text (about the news content); and Label (0 = fake and 1 = real).

There are 78098 data entries in csv file out of which only 72134 entries are accessed as per the data frame.

# What I have done:
The very first step is doing an exploratory data analysis, in which I explored the relationship between labels and features
Compared the data before and after preprocessing, significantly reduced less informative data like punctuations and stopwords
For preprocessing I have used methods like
Lower casing
Removed stopwords,puntuations
Performed Stemming(Finding root words like for functioning root word will be function) using nltk's PorterStemmer
Created sparse matrix using CountVectorizer for vocab size of 6000 features using bag of words and n-grams to extract more details
Train/Test Validation splits
Finally trained models, tuned them to make final predictions

# Model Used:
I have used -> Logistic Regression and find the output
I have coded for Random Forest Regression and KNN Classification but my system was taking too much time to run it, So I have just coded it and didn't run it completely
But the model is correct.

# LIBRARIES used

->scikit-learn
->nltk
->wordcloud
->matplotlib
->seaborn
->pandas
->numpy
