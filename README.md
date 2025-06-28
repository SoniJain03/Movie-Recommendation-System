# Movie Recommendation System

A content-based movie recommendation web app built using **Streamlit** and **cosine similarity algorithm**. 
It recommends similar movies based on selected features like **genres**, **keywords**, **tagline**, **cast**, and **director**.

## Features

- Content-based movie recommendations
- Fast cosine similarity using precomputed matrix
- Efficient vectorizer and model loading with `joblib`
- Interactive UI built with Streamlit

## How it Works

1. Combines selected features (`genres`, `keywords`, `tagline`, `cast`, `director`) into a single text string
2. Transforms the text using `CountVectorizer`
3. Calculates cosine similarity between movies
4. Recommends the top 10 most similar movies to the selected title

## Files & Structure

├── app.py # Main Streamlit application
├── movies.csv # Dataset of movies
├── vectorizer.joblib # Saved CountVectorizer
├── similarity_matrix.joblib # Precomputed cosine similarity matrix
├── requirements.txt # Python dependencies
└── README.md # Project documentation


## Setup Instructions

1. Clone the repository

```bash
git clone https://github.com/your-username/movie-recommender.git
cd movie-recommender

2. Install dependencies

Make sure you have Python ≥3.7 installed
pip install -r requirements.txt

3. Run the app

streamlit run moviemodel.py
