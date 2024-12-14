# Movie Recommendation System

## Introduction
The **Movie Recommendation System** is a machine learning-based project designed to suggest movies to users based on their preferences. This project utilizes collaborative filtering and content-based filtering techniques, using K-Nearest Neighbors (KNN) to predict movie recommendations, enhancing user experience on movie platforms.

## Features
- Personalized movie recommendations.
- Use of KNN algorithm to find similar movies.
- Creation of user-item matrix with sparse representation.
- Analysis of movie statistics (e.g., lowest/highest-rated movies).
- Support for multiple datasets to enrich recommendation accuracy.
- Easy-to-use interface for testing and evaluating recommendations.

## Tech Stack
- **Programming Language**: Python
- **Libraries**: 
  - NumPy
  - Pandas
  - Scikit-learn
  - Matplotlib/Seaborn (for data visualization)
  - SciPy (for sparse matrices)
  - Streamlit (if a web app interface is included)
- **Dataset**: 
  - [MovieLens Dataset](https://grouplens.org/datasets/movielens/)

## How It Works
1. **Data Loading and Preprocessing**:
   - Import movie and rating datasets from provided URLs.
   - Analyze data for key statistics like average ratings per movie and user.
2. **Matrix Creation**:
   - Create a sparse user-item matrix for efficient computation using the SciPy library.
3. **Finding Similar Movies**:
   - Use KNN (K-Nearest Neighbors) to find movies similar to a given movie based on user ratings.
4. **Recommendation for Users**:
   - Identify top-rated movies by a user and suggest similar movies.
5. **Evaluation**:
   - Analyze results to refine the recommendation system.

## Installation
### Prerequisites
- Python 3.7+
- Recommended IDE: Jupyter Notebook, PyCharm, or VS Code.

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Movie-Recommendation-System.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Movie-Recommendation-System
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Run the main script:
   ```bash
   python main.py
   ```
2. Provide user input, such as selecting a movie ID or user ID for recommendations.
3. View the recommended movies in the output.

### Functions Included
- **find_similar_movies(movie_id, X, k)**: Finds movies similar to a given movie ID using KNN.
- **recommend_movies_for_user(user_id, X, user_mapper, movie_mapper, movie_inv_mapper, k)**: Recommends movies for a specific user based on their highest-rated movie.

## Dataset
This project uses the [MovieLens Dataset](https://grouplens.org/datasets/movielens/) for movie and rating data. Ensure the dataset is accessible via URLs or downloaded into the `data` folder before running the project.

## Project Structure
```
Movie-Recommendation-System/
├── data/                 # Dataset folder
├── models/               # Saved models (if applicable)
├── notebooks/            # Jupyter notebooks for development and testing
├── src/                  # Source code for preprocessing, model, and evaluation
├── requirements.txt      # Python dependencies
├── main.py               # Main script to run the system
└── README.md             # Project documentation
```

## Future Enhancements
- Incorporate deep learning models (e.g., neural collaborative filtering).
- Add more user-friendly features like filtering by genre or release year.
- Include additional datasets to improve recommendations.
- Build a robust web application for broader usability.


