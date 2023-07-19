# Sentiment-Analysis
This is a sentiment analysis model that utilizes a dataset containing amazon reviews vs their ratings out of 5 stars.
Any other review vs rating file can also be used, make sure to rename the coloumn heads appropriately.

The code classifies:
5, 4 star reviews as positive
3 star reviews as neutral
1,2 star reviews as negative

Data is preprocessed (made lower case, stop words are removed, lemmatization and non alphabet charachters are removed)
Reviews are then vectorized using TF-IDF vectorizer which assigns numerical value to each word.

test_train_split is used to pass 80% of data as training data and 20% of data as test data

model is created using sklearn's linearSVC model which splits the vectors into the respective divisons( pos,neu and neg)
Model is then analysed using the test data, accuracy is calculated.
Model is then tested using some reviews of our own.
