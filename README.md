# Movie Recommendation System
The system offers personalized suggestions by analyzing plot summaries and metadata (cast, genres, directors). Used advanced techniques like **TF-IDF**, cosine similarity and content-based filtering to process and recommend from a dataset of 5,000+ movies efficiently.

## Execution Guide:


## Overview:
This code implements a **Movie Recommendation System** using content-based filtering. It consists of two main recommendation approaches:

1. **Plot-Based Recommendation**:  
   - Uses the movie plot summaries to compute textual similarities.  
   - A **TF-IDF Vectorizer** transforms the text data into numerical features, and **cosine similarity** identifies closely related movies.  
   - The system recommends movies based on their plot similarity to the user’s input.

2. **Metadata-Based Recommendation**:  
   - Processes movie metadata, including cast, genres, director, and keywords, to create a composite feature called "soup."  
   - Employs a **Count Vectorizer** to analyze categorical similarities and uses **cosine similarity** to identify movies with similar metadata.  
   - Offers recommendations by aligning metadata features.

Additional Highlights:  
- **Weighted Rating**: Computes a weighted rating for movies based on vote count and vote average to filter top-rated movies.  
- **Data Cleaning & Preprocessing**: Handles missing data, parses JSON-like fields (e.g., cast and genres), and standardizes textual data for analysis.  
- **Efficiency**: Processes a dataset of 5,000+ movies and returns top recommendations for the user’s chosen movie.  

This system demonstrates a robust approach to content-based recommendation using text and categorical data.
