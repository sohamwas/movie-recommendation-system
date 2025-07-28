# Movie Recommendation System

## Overview
This Jupyter Notebook implements a content-based movie recommendation system using natural language processing (NLP) techniques. The system analyzes movie metadata (genres, keywords, and overviews) to find similarities between films and suggest relevant recommendations based on a given movie title.

## Key Features
* **Content-Based Filtering:** The system uses movie content features (genres, keywords, and plot summaries) rather than user ratings to make recommendations.
* **TF-IDF Vectorization:** It transforms text data into numerical representations using TF-IDF.
* **Cosine Similarity:** The system measures similarity between movies based on their vectorized features using Cosine Similarity.
* **Data Visualization:** The notebook includes word cloud generation to visualize common terms in movie content.
* **Data Preprocessing:** It handles missing data and combines multiple text features for analysis.

## Dataset
The system utilizes a `movies.csv` dataset containing:
* Movie titles
* Genres
* Keywords
* Plot overviews
* Additional metadata (budget, revenue, cast, crew, etc.)

## Technical Implementation

### Data Loading & Preprocessing
* Loads movie data from CSV.
* Selects relevant features (genres, keywords, overview, title).
* Combines text features into a single column.
* Handles missing values.

### Feature Engineering
* Uses TF-IDF (Term Frequency-Inverse Document Frequency) to vectorize text.
* Computes cosine similarity between movies.

### Visualization
* Generates word clouds to display most common terms in movie content.

### Recommendation Engine
* Finds movies most similar to a given input movie based on combined features.
* For a given movie, the system returns the most similar titles.

## Dependencies
The following Python libraries are required:
* Python 3
* `pandas`
* `numpy`
* `scikit-learn`
* `nltk`
* `wordcloud`
* `matplotlib`

## How It Works
1.  **Data Preprocessing:** The system preprocesses movie data by combining genres, keywords, and overviews.
2.  **TF-IDF Vectorization:** Text data is converted to numerical vectors using TF-IDF.
3.  **Cosine Similarity:** Cosine similarity calculates how similar each movie is to others.
4.  **Recommendation Generation:** For a given movie, the system returns the most similar titles.
