# Movie Recommendation System using Cosine Similarity
This project builds a content-based movie recommender system using cosine similarity to suggest similar titles based on a user’s input. The dataset is provided by YBI Foundation and contains features for each movie.
## Project Workflow
 ### Step 1: Import Required Libraries
- pandas, numpy for data manipulation
- sklearn.metrics.pairwise.cosine_similarity for similarity scoring
- difflib for spelling correction of user input
 ### Step 2: Load Dataset
- Dataset sourced from YBI Foundation
- Movies loaded into a DataFrame with feature-rich metadata
 ### Step 3: Feature Selection
- Text-based or categorical features (e.g. genre, description, cast) selected to define similarity between movies
 ### Step 4: Compute Similarity Score
- Cosine Similarity used to measure pairwise similarity across selected features
- Generates a similarity matrix for all movies
 ### Step 5: User Input and Spelling Validation
- User provides a favorite movie name
- Difflib’s get_close_matches() ensures closest match is selected if there's a typo or variation
 ### Step 6: Recommendation Logic
- Sort all movies based on similarity score to the selected movie
- Top N recommendations returned as output
## Example Use Case
movie_name = input("Enter your favourite movie: ")
## System finds closest match and prints top 10 recommended movies

# Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Difflib
# Outcome
- Personalized movie recommendations
- Handles noisy user input
- Fast, scalable, and interpretable logic using cosine similarity

