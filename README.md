# 🎬 Movie Recommender System

A content-based movie recommendation engine that suggests films similar to ones you enjoy. Built with Python, scikit-learn, and pandas using TF-IDF vectorization and cosine similarity.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [How It Works](#how-it-works)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Technologies](#technologies)
- [Project Structure](#project-structure)

## Overview

This project implements a content-based filtering recommendation system that analyzes movie attributes (genres, keywords, cast, director, and tagline) to find and recommend movies similar to a given movie title. Instead of relying on user ratings, it focuses on the intrinsic features of movies themselves.

## Features

- **Content-Based Filtering**: Recommends movies based on similarity of genres, keywords, cast, director, and tagline
- **TF-IDF Vectorization**: Converts textual movie features into numerical vectors
- **Cosine Similarity Matching**: Calculates similarity scores between movies
- **User-Friendly Input**: Accepts movie titles with fuzzy matching to handle typos and variations
- **Accurate Results**: Returns multiple similar movies ranked by similarity score

## How It Works

1. **Data Loading**: Loads movie metadata from a CSV dataset containing movie information
2. **Feature Selection**: Selects relevant attributes (genres, keywords, tagline, cast, director) for recommendation
3. **Data Preprocessing**: Fills missing values and combines selected features into a single text field
4. **Vectorization**: Converts text features into TF-IDF (Term Frequency-Inverse Document Frequency) vectors
5. **Similarity Calculation**: Computes cosine similarity between the selected movie and all others
6. **Recommendation**: Returns the top N most similar movies

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Pratyush426/movie-recommender.git
   cd movie-recommender
   ```

2. **Install required packages**
   ```bash
   pip install pandas numpy scikit-learn
   ```

3. **Download/Prepare the dataset**
   - Ensure `movies.csv` is in the project directory
   - Dataset should contain columns: `genres`, `keywords`, `tagline`, `cast`, `director`, and movie titles

## Usage

1. Open the Jupyter Notebook:
   ```bash
   jupyter notebook "movie recommender.ipynb"
   ```

2. Run all cells in order to:
   - Load and preprocess the movie dataset
   - Build the recommendation model
   - Enter a movie title when prompted
   - View recommended similar movies

## Dataset

The project uses a movie dataset (CSV format) with the following key columns:
- **genres**: Movie genre(s)
- **keywords**: Associated keywords
- **tagline**: Movie tagline/description
- **cast**: Main cast members
- **director**: Film director(s)

## Technologies

- **Python 3.x**: Programming language
- **pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **scikit-learn**: Machine learning library for TF-IDF and cosine similarity
- **Jupyter Notebook**: Interactive computing environment
- **difflib**: Fuzzy string matching for movie title input

## Project Structure

```
movie-recommender/
├── movie recommender.ipynb    # Main recommendation engine
├── movies.csv                 # Movie dataset
└── README.md                  # Documentation
```

## Author

Created by [Pratyush426](https://github.com/Pratyush426)

---

**Enjoy discovering your next favorite movie! 🍿**
