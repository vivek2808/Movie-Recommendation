# Movie-Recommendation
The Movie Recommendation System presented in this report is designed to provide personalized movie recommendations to users based on their input of a favorite movie. The core technique employed in this system is cosine similarity, The system utilizes a dataset of movies and their associated information to generate recommendations.

Project Implementation Steps:

1.Data Collection:

The project begins with the collection of movie data from a CSV file, including features like genres, keywords, taglines, cast, and directors.
2.Data Preprocessing:

Null values in the selected features are handled by replacing them with empty strings to ensure data completeness.
3.Feature Engineering:

The selected features are combined into a single text representation called "combined_features" to create a comprehensive description of each movie.
4.Text Data to Feature Vectors:

The TfidfVectorizer from scikit-learn is used to convert the text data into numerical feature vectors. This process transforms words into numerical values, resulting in a feature matrix.
Cosine Similarity Calculation:

Cosine similarity is calculated using the feature vectors, resulting in a similarity matrix where each element represents the similarity score between two movies.
5.User Input:

The user is prompted to enter their favorite movie.
6.Finding Close Matches:

The system finds a close match to the user's input within the dataset using the difflib library.
7.Generating Recommendations:

Recommendations are generated by sorting the movies in the dataset based on their similarity scores to the user's input. The top 30 similar movies are displayed to the user.
8.Project Output:
The project provides users with a list of movie recommendations based on their input. It leverages cosine similarity to measure the similarity between movies, enabling the system to suggest movies that align with the user's preferences.

