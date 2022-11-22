# sir-ml-project

Utilized python to implement unsupervised machine learning techniques for a web-based sentiment analysis on oil price for economics planning and scheduling of the refinery operation. 

## Google News scraper and sentiment analyzer using python

Summary:

* Downloads news articles by searching on https://www.google.com/search using URL query parameters.
* Generates CVS files of news text
* Uses pre-trained NLP models to perform sentiment analysis of the news text.


### google_news_scraper.ipynb

* Is a scraper script which can search google news for a given date range using keywords of interest.
* sample data generated by the script looks like this. ( for search query: "oil and gas price")

  ![alt text](https://github.com/Deo-wx/sir-ml-project/blob/main/google_news_data_cleaned.png)

### sentiment_analysis.ipynb

* Takes csv file generated by google_news_scraper.ipynb
* Performs sentiment analysis on each cell
* Performs flair (https://pypi.org/project/flair/), textblob (https://pypi.org/project/textblob/), and VADER (https://www.nltk.org/_modules/nltk/sentiment/vader.html) NLP processing to get sentiment scores.

* Generates sentiment score of each row of text
* Generates descriptive statistics for each metic to get overall sentiment analysis score in the given date range.  

* Sample data generated at this stage looks like this. 

(sentiment_analysis_result.csv)
  ![alt text](https://github.com/Deo-wx/sir-ml-project/sentiment_analysis_result.png?raw=true)

(result_stats.csv)
    ![alt text](https://github.com/Deo-wx/sir-ml-project/result_stats.png?raw=true)


### Credits:
Code from https://github.com/pratikpv/google_news_scraper_and_sentiment_analyzer is used as base to write scraper code.

## Price Prediction
 PASS
