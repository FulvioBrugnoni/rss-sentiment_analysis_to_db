# **News Sentiment Analysis and Storage**

## **Introduction**

This project performs sentiment analysis on news articles fetched from an RSS feed and stores the analyzed data into a PostgreSQL database. The primary goal is to analyze the sentiment of news headlines and manage this data systematically for further analysis.

## **Problem Statement**

The project aims to:
1. **Fetch news articles** from a specified RSS feed.
2. **Analyze the sentiment** of the article titles using text analysis tools.
3. **Store the results**, including sentiment metrics and article details, into a PostgreSQL database for future use.

## **Methodology**

1. **Data Fetching and Preparation:**
   - **Fetch RSS Feed Data:** Utilize the `feedparser` library to fetch and parse the RSS feed.
   - **Prepare Data for Analysis:** Extract relevant details from the feed entries and prepare them for sentiment analysis.

2. **Sentiment Analysis:**
   - **Analyze Article Titles:** Use the `TextBlob` library to compute sentiment scores (polarity and subjectivity) for each article title.
   - **Prepare Data for Storage:** Structure the analyzed data into a list of dictionaries.

3. **Database Interaction:**
   - **Connect to PostgreSQL Database:** Establish a connection to a PostgreSQL database using the `psycopg2` library.
   - **Store Analyzed Data:** Insert the sentiment analysis results along with article details into a designated table in the database.

4. **Error Handling:**
   - **Manage Database Connections:** Handle potential errors in connecting to the database and performing data insertion.

## **Libraries Used**

- **feedparser:** To parse RSS feed data.
- **pandas:** For data manipulation (optional, depending on further analysis).
- **textblob:** For performing sentiment analysis on text.
- **psycopg2:** For PostgreSQL database interaction.
- **datetime:** For date and time operations.


