# Text-Classification
Imported the dataset of 20 new_groups , apply Naive-Bayes on it for Classification and obtain the result.

I need to define some important terms which is used in this classification, which transform text into numeric features:-
1. Count Vectorizer
2. Tf-idf Vectorizer

Count Vectorizer -  It basically creates a dictionary of words from the text corpus. Then, each instance is converted to a vector of numeric features where each element will be the count of the number of times a particular word appears in the document. 

Tf-idf Vectorizer -  It works like the CountVectorizer, but with a more advanced calculation called Term Frequency Inverse Document Frequency (TF-IDF). This is a statistic for measuring the importance of a word in a document or corpus. Intuitively, it looks for words that are more frequent in the current document, compared with their frequency in the whole corpus of documents.

Then we will create a Naïve Bayes classifier that is composed of a feature vectorizer  and the actual Bayes classifier. We will use the MultinomialNB class from the sklearn.naive_bayes module , by using this module we can directly train our model with the Matrix obtained from TF-IDF transformer.

Now we Predict the by using the following steps:-

1. Take your news test data 
2. Again CountVectorize it 
3. Use TD IDF transformer 
4. Then predict it using MultinomialNB()
5. Analyse the result:         
  METRICS.Classification_report()
  Precision 
  Recall 
  F1-score.

Also make the confusion matrix.

