# NLP Sentiment Analysis Practice Exercise

## Overview

This repository contains a practice exercise in Natural Language Processing (NLP), where I explored the application of machine learning models to perform sentiment analysis on the IMDB movie review dataset. The goal of this exercise was to classify movie reviews as either positive or negative based on their content.

## Project Structure

- **`IMDB Dataset.csv`**: The dataset used for the exercise, containing movie reviews and their associated sentiment labels. (https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews?resource=download)
- **`NLP - Bags Of Words.ipynb`**: The Jupyter Notebook where the analysis and model training were performed.
- **`requirements.txt`**: A list of Python dependencies required to run the notebook.

## Methodology

1. **Data Preprocessing**:
   - Loaded the IMDB dataset.
   - Converted the text reviews into numerical features using the Bag-of-Words approach.
   - Labeled the sentiment as `1` for positive reviews and `0` for negative reviews.

2. **Model Training**:
   - Experimented with three different models:
     - **K-Nearest Neighbors (KNN)**
     - **RandomForest**
     - **Multinomial Naive Bayes (MultinomialNB)**
   - Split the data into training and testing sets to evaluate the performance of each model.

3. **Evaluation**:
   - Compared the models based on accuracy, precision, recall, and F1-score.
   - Analyzed why KNN struggled with this high-dimensional text data compared to RandomForest and MultinomialNB.

## Key Insights

- **K-Nearest Neighbors (KNN)**: This model struggled with the high-dimensional nature of text data, leading to poor performance in sentiment classification.
- **RandomForest and MultinomialNB**: Both models outperformed KNN, with RandomForest capturing complex patterns through its ensemble approach and MultinomialNB effectively handling the categorical nature of word features.

