# Movie Recommendation System

This project is a simple content-based recommendation system for movies. It uses genres as features to find similar movies based on cosine similarity.

## How to Use
1. Install dependencies: `pip install -r requirements.txt`
2. Run the app: `python app.py`
3. Access the API at `http://127.0.0.1:5000/recommend?title=<MOVIE_TITLE>`

## Features
- Content-based filtering using TF-IDF on genres
- Flask API for easy deployment

## Example
Request recommendations for "Toy Story (1995)":

**Request:**  
`http://127.0.0.1:5000/recommend?title=Toy%20Story%20(1995)`

**Response:**  
```json
[
    {"title": "A Bug's Life (1998)", "genres": "Adventure|Animation|Children|Comedy|Fantasy"},
    {"title": "Toy Story 2 (1999)", "genres": "Adventure|Animation|Children|Comedy|Fantasy"},
    ...
]
