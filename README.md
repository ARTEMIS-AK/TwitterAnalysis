# Twitter Sentiment Analysis

This project focuses on sentiment analysis of tweets using natural language processing (NLP) techniques and machine learning algorithms. The analysis includes cleaning the text data, extracting sentiment scores, and summarizing the overall sentiment of the dataset.

## Project Description

### Data Loading and Preprocessing
1. **Data Loading**: The dataset is loaded using pandas from a CSV file named `emotions.csv`.
2. **Text Cleaning**: The text data is cleaned using a custom function that:
    - Converts text to lowercase.
    - Removes HTML tags, URLs, punctuation, and numerical values.
    - Eliminates stop words (common words that are usually not meaningful in analysis).
    - Applies stemming to reduce words to their root form.

### Sentiment Analysis
1. **Sentiment Scoring**: The sentiment of each tweet is analyzed using the `SentimentIntensityAnalyzer` from the NLTK library. Three sentiment scores are extracted for each tweet:
    - **Positive**: Indicates the proportion of positive sentiment.
    - **Negative**: Indicates the proportion of negative sentiment.
    - **Neutral**: Indicates the proportion of neutral sentiment.
2. **Data Aggregation**: The dataset is filtered to include only the tweets and their respective sentiment scores.

### Sentiment Summary
1. **Score Summation**: The total positive, negative, and neutral scores are calculated.
2. **Sentiment Determination**: A function `sentiment_score` is used to determine the overall sentiment of the dataset based on the highest cumulative score.

### Results
The script prints the cumulative positive, negative, and neutral scores and indicates that the overall sentiment of the dataset is neutral.

## Dependencies
- pandas
- numpy
- scikit-learn
- nltk

This project provides a foundation for analyzing sentiments in textual data and can be extended to include more sophisticated machine learning models and additional data preprocessing techniques.
