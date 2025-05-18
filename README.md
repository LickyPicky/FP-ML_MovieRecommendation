# Movie Recommendation System 

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
<!-- You can add a badge for Jupyter if you like: ![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg) -->

## Description
This project implements a movie recommendation system that suggests movies to users based on their past rating behavior. It leverages collaborative filtering techniques to predict user preferences and generate personalized recommendations

## Why This Project?
This movie recommendation system was developed as the **Final Project for the Machine Learning course (CSAC 224) at Camarines Sur Polytechnic Colleges.**

## Features
*   Predicts movie ratings for users.
*   Generates Top-N movie recommendations for a specified user.
*   Evaluates model performance using metrics such as RMSE, Precision@10, Recall@10, and F1-score@10.
*   Demonstrates the application of Singular Value Decomposition (SVD) for recommendation tasks.

## Technologies Used
*   **Python 3.x**
*   **Jupyter Notebook:** For demonstration, analysis, and presentation of the system.
*   **Pandas:** For data loading, manipulation, and analysis.
*   **NumPy:** For numerical operations.
*   ** `Surprise` library, `Scikit-learn` library for SVD.
*   **Matplotlib / Seaborn (Optional):** If used for visualizations within the notebook.

## Dataset
This system is trained and evaluated on the **MovieLens 32M, a custom subset of TMDB**.
*   **Source:** (https://grouplens.org/datasets/movielens/)
*   **Files Included:**
    *   `ratings.csv` - Contains user ratings for movies.
    *   `movies.csv` - Contains movie metadata like titles and genres.
    *   `tags.csv` - Contains movie tags.
*   **Description:** MovieLens 32M movie ratings. Stable benchmark dataset. 32 million ratings and two million tag applications applied to 87,585 movies by 200,948 users. Collected 10/2023 Released 05/2024.

## Repository Contents
This repository contains:
1.  **`MovieRecommend.ipynb`**: The main Jupyter Notebook demonstrating the entire movie recommendation process, from data loading and preprocessing to model training, evaluation, and generating recommendations.
2.  **`data/` directory (or similar)**: Containing the necessary CSV files:
    *   `ratings.csv`
    *   `movies.csv`
    *   `tags.csv`
3.  **`README.md`**: This file.

## Usage
To view and run the movie recommendation system:
1.  Ensure you have Python and Jupyter Notebook installed on your system.
2.  Download or clone this repository.
3.  Navigate to the repository's directory in your terminal.
4.  Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
5.  Open the `MovieRecommend.ipynb` file from the Jupyter Notebook interface in your browser.
6.  You can then run the cells in the notebook sequentially to see the system in action.

**Note:** This project is primarily for demonstration within the Jupyter Notebook environment. Guidance for local installation or deployment as a standalone application is not provided.

## Example Output / Results (from the Notebook)

The system's performance metrics on the test set, as demonstrated in the notebook, are:
*   **RMSE:** 0.7717
*   **RMSE on test set (more precise):** 0.7717007704524537
*   **Precision@10 (threshold=3.5):** 0.8120
*   **Recall@10 (threshold=3.5):** 0.5714
*   **F1-score@10 (threshold=3.5):** 0.6708

An example recommendation for User ID 18:
*   **Context (User's Top Rated):** American Beauty (5.0), Big Lebowski (5.0), etc.
*   **Top Recommendations:** Decalogue (Pred: 4.90), Wizard of Oz (Pred: 4.88), etc.


## How It Works (Briefly - as demonstrated in the Notebook)
The recommendation logic implemented in the notebook is based on User-Based Collaborative Filtering using  Matrix Factorization (SVD).

- *Collaborative Filtering:* The notebook demonstrates finding users similar to a target user based on their rating patterns and then recommends items liked by these similar users.
- *Matrix Factorization (like SVD):* The notebook shows how the user-item interaction matrix is decomposed into latent factor matrices to predict missing ratings.]
