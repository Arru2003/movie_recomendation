
# Movie Recommendation System using Content-Based Filtering

## Overview
This Python script implements a movie recommendation system based on content-based filtering techniques. The system suggests movies similar to a user's input movie by analyzing textual features such as genres, keywords, tagline, cast, and director.

## Prerequisites
Before running the script, ensure you have the following dependencies installed:
- `numpy`
- `pandas`
- `scikit-learn`
- `difflib`

You can install these dependencies using pip:
```
pip install numpy pandas scikit-learn
```

## Usage
1. **Data Preparation**: 
   - Prepare a movie dataset in CSV format containing features like genres, keywords, tagline, cast, director, etc.
   
2. **Running the Script**:
   - Import necessary libraries.
   - Read the movie dataset using `pd.read_csv()`.
   - Select relevant features for analysis (e.g., genres, keywords, etc.).
   - Handle missing values in selected features.
   - Combine selected features into a single text representation.
   - Use TF-IDF vectorization to convert text data into numerical values.
   - Calculate cosine similarity between movies based on feature vectors.
   - Take user input for their favorite movie.
   - Find the closest match to the user's input movie.
   - Retrieve similarity scores for recommended movies.
   - Display recommended movies sorted by similarity score.

3. **Input**:
   - When prompted, enter the name of your favorite movie.

4. **Output**:
   - The script will suggest a list of movies similar to the user's input movie based on content features.

## Example
Here's how you can use the script:
```bash
python movie_recommendation.py
```
Enter the name of your favorite movie when prompted, and the script will suggest similar movies based on content features.

## Note
- This script demonstrates a basic content-based filtering approach for movie recommendation. For more advanced recommendation systems, consider collaborative filtering, matrix factorization, or neural network-based models.
