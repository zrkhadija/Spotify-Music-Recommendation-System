# Music Recommendation System (Hybrid Content-Based + LLM) 🎶
## Project Overview

This project implements an advanced music recommendation system using the Spotify dataset. The system combines audio feature analysis with semantic embeddings from song titles and artists to provide personalized, content-based recommendations. It’s designed to demonstrate expertise in data preprocessing, feature engineering, machine learning, and natural language processing with LLMs.

## The system demonstrates expertise in:

>Data preprocessing and feature engineering

>Machine learning for recommendation systems

>Natural language processing with LLMs

> Data visualization for interpretation

## Dataset

>> Source: Kaggle Spotify datasets (data.csv)

>>Number of songs: 170,653

>> Features include:

>> Numeric/audio: valence, danceability, energy, popularity, tempo, explicit, mode, key

>> Categorical: artist_encoded

>> Text: name + artist for LLM embeddings

# Key Steps
## Exploratory Data Analysis (EDA)

>Visualized distributions of audio features

>Performed correlation analysis

>Analyzed popularity trends over time

>Explored genre and artist insights

## Data Preprocessing

>Scaled numeric features using StandardScaler

>Encoded artists

>Extracted song text for embeddings (name + artist)

>Handled missing values and performed feature engineering (month, decade)

>LLM Integration

>Used SentenceTransformers (all-MiniLM-L6-v2) to generate semantic embeddings

>Combined embeddings with numeric/audio features to create a hybrid feature matrix

## Recommendation Engine

>Implemented NearestNeighbors (cosine similarity) for retrieval

>Weighted numeric/audio features and LLM embeddings

>Created a recommendation function returning top-N similar songs

## Visualization

>Generated radar charts to compare features between query song and recommendations

>Analyzed diversity, popularity, and similarity of recommended songs

## Evaluation

>Cosine similarity scores between recommended songs

>Diversity of recommended songs (audio features)

>Popularity bias analysis
