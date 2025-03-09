
# News Sentiment Analysis System

## Description
A news sentiment analysis platform that fetches news articles using the Bing News Search API, analyzes sentiment, and categorizes articles based on sentiment scores. The system helps users understand the emotional tone of news articles, providing insights into media trends.

## Features
- Fetches real-time news from Bing News API
- Sentiment analysis using NLP models (TextBlob, VADER, FinBERT)
- Displays structured sentiment-based insights
- Categorizes news as positive, negative, or neutral
- Graphical representation of sentiment trends over time

## Technologies Used
- **Backend:** Flask (Python)
- **Frontend:** React.js
- **Sentiment Analysis:** TextBlob, VADER, FinBERT
- **Database:** PostgreSQL
- **Data Visualization:** Chart.js

## Challenges Faced & Solutions
- **Issue:** Handling large volumes of news data
  - **Solution:** Implemented efficient data storage and indexing
- **Issue:** Ensuring accurate sentiment classification
  - **Solution:** Tuned NLP models and improved feature extraction