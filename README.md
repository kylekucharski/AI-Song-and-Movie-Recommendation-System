# S.a.M - CS 450 Final Project

## Overview
Recommendation systems have become an essential part of our daily lives. With the exponential expansion of readily available media, it can be difficult to expand your taste. Many of the applications we use today have their own algorithms to sort content and present what they think you'll like. We created S.a.M, the AI-enhanced **S**ong **a**nd **M**ovie recommendation system to help expand your interests. Just provide it with one song or movie you already like, and S.A.M will give you 10 recommendations using our algorithms.

## Project Goals
The goal of the project was to explore recommendation system mechanics and compare the effectiveness of different machine-learning techniques. We wanted to see how different algorithms personalize content recommendations. To do so, we developed specialized algorithms for both songs and movies. 

## Core Concepts Used
* Content-Based Filtering: Uses item features to recommend similar items based on previous actions or explicit feedback
* K-Means Clustering: Partitions data into K clusters in which each data point belongs to the cluster with the nearest mean
* Euclidean Distance: Calculates the distance between two data points using the square root of the sum of the square differences
* Principal Component Analysis: Dimensionality reduction method used to simplify a large data set into a smaller one while maintaining significant patterns and trends

## Getting Started
To get S.a.M running on your local machine, follow the steps below.

### Installing Dependencies
Before we begin, you will need to have Python 3.10+ installed on your machine. You can download it [here](https://www.python.org/downloads/). It is encouraged to use Anaconda as it has NumPy preinstalled. Otherwise, install instructions can be found below.

Now that Python has been installed, we will need to install the Pandas, NumPy, and Jupyter Notebooks. You can use the following code in the Anaconda terminal:

To install Pandas:
`pip install pandas`

To Install NumPy:
`pip install numpy`

To Install Jupyter Notebooks:
`pip install jupyter`

### Downloading The Files
Now we can set up the project. You will need to download the following:
* [S.aM.ipynb](docs/S.aM.ipynb)
* [Dataset.csv](docs/dataset.csv)
* [Movies.csv](docs/movies.csv)
* [Ratings.csv](docs/ratings.csv)

### Final Steps
Now that we have everything installed and downloaded, you can use your desired Python environment to open the project files and begin running your own S.a.M! 

## Usage
The recommendation system can be run directly through the Jupyter Notebook file. 
For song recommendations, at _In[21]_, run the following code:
`get_euclidean_recommendations('Song Title of Your Choice', features, df, final_df)`
S.a.M will then give you 10 songs it thinks you'll like!

For Movie Recommendations, at _In[44]_, run the following code:
`get_content_recommendations('Movie Title of Your Choice', cosine_similarity_matrix)`
S.a.M will then give you 10 movies it thinks you will like!

**Note: Inputs are limited to the songs and movies included in the dataset**

If you choose to implement the system into you're own program, there is a `show_menu()` function that lets the user choose what to do. This will invoke the appropriate methods for either song or movie recommendations, or throw an error if the Title is not found in our dataset. 

## References and Sources
* [Spotify Tracks Dataset](https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset?resource=download)
* [TMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata/data)
* [Build Personal Playlists With Machine Learning](https://www.sciencebuddies.org/science-fair-projects/project-ideas/ArtificialIntelligence_p012/artificial-intelligence/K-Means-Spotify)

### Licenses
[Database: Open Database, Contents: &copy; Original Authors](http://opendatacommons.org/licenses/odbl/1.0/)
