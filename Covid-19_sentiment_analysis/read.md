# Installation and the usage of TextBlob: a sentiment analysis tool
For this project, we use [Textblob](https://github.com/sloria/TextBlob) to do sentiment analysis.

It is a high star project on github.

We use it as it is a fast-speed and easy-installation library.

## Installation
```
$ pip install -U textblob
$ python -m textblob.download_corpora
```

For those in China, please use vpn when downloading nltk corpora.

## Usage
```
$ from textblob import TextBlob
$ text = '''text'''
$ blob = TextBlob(text)

$ blob.sentiment
Sentiment(polarity=0.39166666666666666, subjectivity=0.4357142857142857)
$ lbob.sentiment.polarity
0.39166666666666666
```
The sentiment property returns a namedtuple of the form Sentiment(polarity, subjectivity). The polarity score is a float within the range [-1.0, 1.0]. The subjectivity is a float within the range [0.0, 1.0] where 0.0 is very objective and 1.0 is very subjective.
