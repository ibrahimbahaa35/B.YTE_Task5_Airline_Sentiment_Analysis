# B.YTE_Task5_Airline_Sentiment_Analysis
# Social Media Sentiment Analysis — Twitter US Airline Sentiment

## 1. Project Overview
This project fulfills **Task 5 — Social Media Sentiment Analysis (Basic)**. It involves analyzing tweet-length social media posts to uncover customer sentiment trends. The pipeline includes comprehensive exploratory data analysis (EDA), natural language text preprocessing, sentiment polarity classification, and data visualization to derive business-driven actionable insights.

## 2. Dataset Information
- **Dataset Name:** Twitter US Airline Sentiment
- **Source:** [Kaggle - Twitter US Airline Sentiment](https://www.kaggle.com/datasets/crowdflower/twitter-airline-sentiment)
- **Collection Date:** February 2015
- **Description:** A dataset of 14,640 tweets classifying customer feedback for major US airlines. Key attributes utilized include `text`, `airline_sentiment`, `negativereason`, and `tweet_location`.

## 3. Methodology & Text Preprocessing
The raw tweet data was cleaned and transformed for analysis using the following Natural Language Processing (NLP) techniques:
- **Noise Removal:** Applied Regular Expressions (Regex) to strip out URLs, `RT` (retweet) tags, and hashtag symbols (`#`).
- **Tokenization:** Utilized NLTK's `TweetTokenizer` to split text into distinct word tokens while lowercasing and stripping user handles (`@`).
- **Stop-Word & Punctuation Filtering:** Removed standard English stopwords (via NLTK corpus) and punctuation to focus on meaningful vocabulary.
- **Stemming:** Applied the `PorterStemmer` to reduce words to their base root forms.
- **Polarity Computation:** Used `TextBlob` to calculate sentiment polarity scores and classify the cleaned text into `positive`, `negative`, or `neutral` categories.

## 4. Visualizations Required
The analysis produces the following key visual deliverables (saved as images in the repository):
- **Sentiment Distribution Bar Chart:** A Seaborn countplot illustrating the distribution of the sentiment classes, revealing the data's lean toward negative customer feedback.
- **Sentiment Word Clouds:** Generated visualizations (`WordCloud`) for the Positive, Neutral, and Negative sentiment classes to highlight the most frequent terms driving each category.

## 5. Actionable Insight Summary
**Key Findings & Recommendation:**

The sentiment analysis reveals a high level of customer dissatisfaction, primarily driven by operational failures like flight delays, cancellations, and lost luggage. Meanwhile, the neutral sentiment word cloud highlights passengers actively seeking customer support, with frequent terms like "help," "DM," and "please". 

**Actionable Insight:** Airlines must prioritize resolving operational bottlenecks, particularly baggage handling and on-time performance. Additionally, empowering social media teams to proactively assist with rebooking and provide real-time updates can significantly convert negative interactions into positive customer experiences.
