# bharat_intern_MOVIE-RECOMMENDATION-SYSTEM


This project involves building a movie recommendation system using a dataset of movies. The system suggests movies to users based on their similarity to a movie the user likes. This is achieved using Natural Language Processing (NLP) techniques and cosine similarity.

Tools and Technologies Implemented

Python: The programming language used for this project.

Pandas: A powerful data manipulation library used for loading and processing the dataset.

NumPy: A library used for numerical computations.

Scikit-learn: A machine learning library used for vectorizing text data and calculating cosine similarity.

Difflib: A Python module for comparing sequences, used here to find close matches for movie titles.



Concepts Used

Data Preprocessing:

Loading Data: The dataset is loaded into a Pandas DataFrame.

Handling Missing Values: Missing values in selected features are filled with empty strings to avoid errors during text processing.

Feature Selection:

The relevant features for the recommendation system are selected: genres, keywords, tagline, cast, and director. These features provide a comprehensive description of the movies.

Combining Features:

The selected features are combined into a single string for each movie to form a comprehensive text description.

Text Vectorization:

TF-IDF Vectorization: The combined text descriptions are converted into numerical feature vectors using the TF-IDF (Term Frequency-Inverse Document Frequency) Vectorizer. This step transforms text data into a format suitable for calculating similarity.

Cosine Similarity:

Cosine Similarity Calculation: Cosine similarity is used to measure the similarity between the feature vectors. It calculates the cosine of the angle between two vectors, giving a similarity score between 0 and 1.

Finding Close Matches:

Difflib: Used to find the closest match for a user's input movie name from the list of all movie titles in the dataset.

Recommendation Generation:

Index Matching: The index of the user's input movie is found, and the similarity scores for all other movies are retrieved.

Sorting: The movies are sorted based on their similarity scores in descending order.

Top Recommendations: The top similar movies are presented to the user as recommendations.

Code Breakdown

Importing Dependencies:

Libraries are imported for data manipulation, text vectorization, and similarity calculations.

Data Collection and Preprocessing:

The movie dataset is loaded, and missing values in selected features are handled.

Feature Combination:

The selected features are combined into a single text string for each movie.

Text Vectorization and Similarity Calculation:

The combined text data is vectorized using TF-IDF.

Cosine similarity is calculated between the feature vectors of all movies.

User Input and Recommendation:

The user is prompted to enter their favorite movie.

The closest match for the movie title is found.

The index of the matched movie is used to retrieve similarity scores.

The movies are sorted based on similarity scores, and the top recommendations are displayed to the user.

Insights


Data Quality: Ensuring data completeness and correctness is crucial for accurate recommendations.

Feature Engineering: Combining relevant features into a single text string allows for a more comprehensive representation of each movie.

Similarity Metrics: Cosine similarity is effective in comparing text data and providing meaningful recommendations.

User Experience: Finding close matches for user input improves the user experience by handling variations in movie title input.

This project demonstrates the application of NLP techniques and similarity metrics in building a recommendation system, showcasing the integration of multiple libraries and concepts to deliver a functional solution.
