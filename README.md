# User-Based Movie Recommendation System

## Project Structure
- `movies.csv` : Movie dataset
- `ratings.csv` : User ratings dataset
- `main.ipynb` : Main project implementation
- `README.md` : Project documentation
- `LICENSE` : License information

## Project Overview

In this project, a **User-Based Collaborative Filtering** recommendation system was implemented to suggest movies to a new user based on their ratings and similarities with other users.

## Implementation Steps

### 1. Data Preprocessing
- Organized the `movies` and `ratings` DataFrames.
- Removed unnecessary columns.
- Cleaned and standardized movie titles using Regular Expressions (Regex).

### 2. New User Input
- Created a hypothetical user input containing movie ratings.
- Used this input to simulate a new user and test the recommendation system.

### 3. User Filtering
- Extracted ratings from users who had watched at least one of the movies rated by the new user.
- Further filtered the dataset to identify users who had watched and rated **all movies** rated by the new user.

### 4. Similarity Calculation
- Used **Pearson Correlation** to calculate the similarity between the new user and other users.
- Compared users based on their ratings for the same movies.

### 5. Movie Recommendation
- Applied the calculated similarity scores as weights to movie ratings.
- Ranked movies based on their weighted similarity scores.
- Recommended movies with the highest scores to the new user.

## Algorithm
- User-Based Collaborative Filtering
- Pearson Correlation

## Technologies
- Python
- Pandas
- NumPy
- Regular Expressions (Regex)
- Jupyter Notebook
