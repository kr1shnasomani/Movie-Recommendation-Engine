# Movie Recommendation System
The system offers personalized suggestions by analyzing plot summaries and metadata (cast, genres, directors). Used advanced techniques like **TF-IDF**, cosine similarity and content-based filtering to process and recommend from a dataset of 5,000+ movies efficiently.

## Execution Guide:
1. Run the following command line in the terminal:
   ```bash
   pip install numpy pandas matplotlib scikit-learn
   ```
2. Download the dataset (link to the dataset: **https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata**)

3. Copy paste the path of the `tmdb_5000_movies.csv` and `tmdb_5000_credits.csv` files in the code

4. Enter the movie name whose recommendation you want in the `user_movie` cell

5. There are two types of recommendation which you can get. One is based on the plot and the other one based on the metadata

6. The following images shows how the output will look like:

   ![image](https://github.com/user-attachments/assets/2de1d762-fade-4285-ab3e-578e184ca808)

   ![image](https://github.com/user-attachments/assets/27b22fae-77d4-4146-9218-e1ba16b9d122)

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
