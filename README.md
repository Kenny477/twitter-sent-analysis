# Sentiment Analyzer from Twitter Cashtags

This Python script pulls data from Twitter using the Twint library. The data is cleaned, then fed into a Naive Bayes classifier that was previously trained from a sample tweet dataset.

### Sentiment Score

The sentiment score for each stock is calculated through a simple averaging algorithm.
"Positive" = 1
"Negative" = -1
The scores for the number of tweets selected are added up and averaged. Positive average means overall positive sentiment and vice versa.

### Accuracy

The accuracy of the sentiment scores is proportional to the number of tweets for each stock pulled.

For example: 1000 tweets/stock results in a sentiment score to the 1/1000th place.

### Future Improvements

1. Improve time complexity by checking if the data exists beforehand.
2. Modify classifier to output numerical sentiment scores rather than "Positive" or "Negative".
3. Find a more complex algorithm to convert binary values into a decimal sentiment score.\

### Credits

Twint tutorial from [Medium](https://medium.com/analytics-vidhya/how-to-scrape-tweets-from-twitter-with-python-twint-83b4c70c5536)

NLTK Sentiment Analysis tutorial from [Digital Ocean](https://www.digitalocean.com/community/tutorials/how-to-perform-sentiment-analysis-in-python-3-using-the-natural-language-toolkit-nltk)
