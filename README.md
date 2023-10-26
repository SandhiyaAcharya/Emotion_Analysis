# NLP Emotion Analysis

This repository contains code for performing emotion analysis on text data using Natural Language Processing (NLP) techniques. The dataset used for this project is sourced from [Data World](https://data.world/crowdflower/sentiment-analysis-in-text) and consists of tweets labeled with emotions.

## About the Dataset

The dataset contains four columns: `twitter_id`, `author`, `content`, and `emotion`. It includes labels for the emotional content (e.g., happiness, sadness, anger) of texts. There are hundreds to thousands of examples across 13 different emotion labels.

## Project Overview

1. **Data Cleaning**
   - Renamed the column "sentiment" to "emotion".
   - Removed empty string entries from the "emotion" column.
   - Eliminated rows with zeros in the "content" column.

2. **Data Visualization**
   - Conducted a countplot on the "emotion" column to visualize the frequency of each emotion category.

3. **Vaex Library for Handling Large Data**
   - Utilized Vaex for efficient handling of large-scale data due to its memory-mapping and lazy-loading capabilities.

4. **Text Processing**
   - Lowercased all text for uniformity.
   - Handled HTML tags, emojis, emails, and URLs.
   - Removed special characters, numbers, and punctuation.
   - Expanded contractions and corrected misspelled words.
   - Removed stopwords and tokenized the text.
   - Applied lemmatization to reduce words to their base form.

## Usage

To run the code, follow these steps:

1. Install the necessary libraries and packages.
2. Load the dataset using `pd.read_csv()`.
3. Follow the data preprocessing steps outlined in the code.
4. Use the processed data for your emotion analysis task.

## References

- [Data World - Sentiment Analysis in Text](https://data.world/crowdflower/sentiment-analysis-in-text)

