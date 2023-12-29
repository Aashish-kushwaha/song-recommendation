# Song Recommendation System

## Overview

This project implements a song recommendation system based on the content of song lyrics. The system utilizes Natural Language Processing (NLP) techniques to analyze and process song lyrics, and then employs cosine similarity along with TF-IDF vectorization to recommend songs that are similar in content.

## Data

The project uses a dataset (`songdata.csv`) containing song lyrics. The data preprocessing involves cleaning the text data, removing special characters, converting text to lowercase, and performing tokenization and stemming using NLTK.

## Methodology

1. **Data Preprocessing**: The initial dataset is cleaned and reduced to a sample of 5000 rows.

2. **Text Processing**: Song lyrics are tokenized, and stemming is applied to reduce words to their base form.

3. **TF-IDF Vectorization**: The lyrics are converted into TF-IDF vectors, capturing the importance of each word in the corpus.

4. **Cosine Similarity**: Cosine similarity is used to measure the similarity between songs based on their TF-IDF vectors.

5. **Recommendation Function**: A recommendation function is implemented to suggest songs similar to a given input song.

## Project Structure

- `app.py`: Flask web application with two routes for displaying song names and handling song recommendations.
- `df.pkl`: Pickle file storing the preprocessed DataFrame.
- `similarity.pkl`: Pickle file storing the cosine similarity matrix.
- `main.ipynb`: Jupyter Notebook containing the main code for the song recommendation system.
- `recommendation_module.py`: Python script with the recommendation function.
- `songdata.csv`: Dataset containing song lyrics.