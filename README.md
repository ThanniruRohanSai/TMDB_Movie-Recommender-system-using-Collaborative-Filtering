# TMDB_Movie-Recommender-system-using-Collaborative-Filtering
This project builds a movie recommender system using Collaborative Filtering techniques to suggest relevant movies to users based on their past preferences.

Data:

The project utilizes the publicly available TMDB (The Movie Database) movie ratings dataset. This dataset can be found on various online platforms, including https://www.kaggle.com/datasets/grouplens/movielens-20m-dataset.

Method:

Collaborative Filtering (CF) is a recommendation technique that analyzes user-movie rating patterns to identify users with similar tastes. Based on these similarities, the system recommends movies that users with similar preferences have enjoyed.

This project implements a Matrix Factorization (MF) approach for Collaborative Filtering:

Data Preprocessing: The dataset is loaded and cleaned to handle missing values and inconsistencies.
User-Movie Rating Matrix: A user-movie rating matrix is constructed where rows represent users and columns represent movies. The cell values correspond to the user's rating for a specific movie (if available).
Matrix Factorization: The user-movie rating matrix is decomposed into two lower-dimensional matrices. One matrix represents latent factors describing user preferences, and the other represents latent factors describing movie characteristics.
Recommendation Generation: For a target user, the system utilizes the user's latent factors and the movie latent factors to predict potential ratings for unrated movies. Movies with the highest predicted ratings are recommended to the user.
Note: Due to size limitations, the pre-trained model and the "credits.csv" file from the dataset are not included. However, the code provided focuses on building the recommendation system using collaborative filtering principles.

Evaluation:

The performance of the recommender system can be evaluated using various metrics. Potential metrics include:

Precision: Measures the accuracy of recommendations, indicating the proportion of recommended movies that the user actually enjoys.
Recall: Measures the completeness of recommendations, indicating the proportion of movies the user might enjoy that are actually recommended by the system.
Normalized Discounted Cumulative Gain (NDCG): Evaluates the ranking quality of recommendations, considering the relevance and order of recommended movies.

Future Work:

Explore alternative recommendation techniques like Content-Based Filtering or Hybrid approaches that combine CF and CBF.
Implement advanced Matrix Factorization methods like SVD++ or NMF for potentially improved performance.
Incorporate user information beyond ratings, such as genres, directors, or actors, to personalize recommendations further.
Integrate the recommender system into a user interface for easy movie exploration and discovery.
