## Fadhillah-Rojabhy_Project1 - Sentiment Analysis on Indonesian Presidential Election Tweets

# Background
This project focuses on analyzing sentiments from tweets during the 2019 Indonesian Presidential Election. The dataset consists of 1,815 tweets, which are categorized into three sentiments: positive, neutral, and negative. The aim is to leverage machine learning algorithms to classify and understand public sentiment during this critical period.

# Objective
The main goal is to develop and compare the performance of two machine learning models—Random Forest and Long Short-Term Memory (LSTM)—to classify the sentiment of the tweets accurately. The project seeks to identify which model offers better performance in sentiment classification.

# Key Steps:
1. Data Preprocessing: Lowercase conversion, Emoji handling, Removal of hashtags, mentions, URLs, Stopword removal (with exceptions), Slang word normalization, Stemming using Sastrawi
2. Feature Extraction: TF-IDF vectorization
3. Model Development: Random Forest classifier, LSTM neural network
4. Hyperparameter Tuning: GridSearchCV for Random Forest

# Results:
1. Random Forest:
Best parameters: max_depth=20, min_samples_split=5, n_estimators=300
Test accuracy: 62%
Balanced performance across classes (precision, recall, f1-score around 0.62)
2. LSTM:
Test accuracy: 55.65%
Shows signs of overfitting (training accuracy reaches 98% while validation stays around 55%)

# Summary:
This project demonstrates the application of NLP techniques for Indonesian language processing and sentiment analysis of political tweets. The Random Forest model slightly outperformed the LSTM model, possibly due to the limited dataset size. The preprocessing steps, including emoji handling and slang word normalization, were crucial for adapting to the nuances of Indonesian social media text.

# Future work could focus on:
1. Gathering more data to improve model performance
2. Experimenting with more advanced deep learning architectures
3. Exploring ensemble methods combining multiple models
4. Further refining preprocessing techniques for Indonesian text

