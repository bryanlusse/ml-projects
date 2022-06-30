<div align="center">

# Movie Recommendation on The Movie Dataset

![Badge](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white)

![Badge](https://img.shields.io/github/languages/code-size/bryanlusse/ml-projects)
![Badge](https://img.shields.io/github/languages/count/bryanlusse/ml-projects)
![Badge](https://img.shields.io/github/last-commit/bryanlusse/ml-projects)

[Overview](#scroll-overview)
•
[Models](#chart_with_upwards_trend-model)
•
[Results](#closedbook-results)
</div>

## :bookmark_tabs: Menu

- [Overview](#scroll-overview)
- [Models](#chart_with_upwards_trend-model)
- [Requirements](#exclamation-requirements)
- [Folder Structure](#closedbook-results)
- [Results](#open_file_folder-folder-structure)
- [Author](#smiley_cat-author)

## :scroll: Overview

This folder hosts a projects that performs movie recommendation on a dataset of movies. The data comes from [The Movies Dataset](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset), which contains information on approximately 45,000 movies from 2017 and before obtained from [MovieLens](https://grouplens.org/datasets/movielens/) and [TMDB](https://www.themoviedb.org/?language=nl).

The notebook can be accesed on Google Colab through this [link](https://drive.google.com/file/d/1j2JjiJLFcfRArl5IGFwfE5EfWiX4EY8T/view?usp=sharing)

Recommendation algorithms can be used in a large variety of fields. Recommendations can be based on content similarities, user interest similarities, demographics or general popularity. 

## :carpentry_saw: Preprocessing

For the content-based model preprocessing of the data was done using standard text preprocessing methods: Removal of stopwords and punctuation.
Afterwards, vectorization was performed using multiple methods:
- Bag of Words
- Term Frequency - Inverse Document Frequency (TF-IDF) 
- Word2Vec

## :chart_with_upwards_trend: Models

A content-based algorithm was constructed using the Cosine Similarity to calculate the similarity of movies. Additionally, a second collaborative model consisting of a Singular Value Decomposition (SVD) algorithm was created in order to make recommendations based on user ratings.

## :closed_book: Results

All methods succeeded in predicting relevant movie recommendations. From the two methods, not one can easily be called superior to the other. Recommendation systems in industry base their recommendations on multiple factors, so ideally, methods should be combined in order to give the most accurate recommendations.

For the content-based algorithm we did notice that using Word2Vec vectorization lead to less accurate results.

## :exclamation: Requirements

Found in [requirements.txt](https://github.com/bryanlusse/ml-projects/blob/master/movie-recommendations/requirements.txt).


## :open_file_folder: Folder Structure

```
.
├── data                                     # Movie dataset
├── assets                                   # Images for notebook
├── Movie_Recommendation.ipynb               # Main notebook
├── iframe_figures                           # Plots of words in clusters
├── requirements.txt                         # Required packages
├── svd.pickle                               # SVD model
└── README.md
```

## :smiley_cat: Author

- [@bryanlusse](https://github.com/bryanlusse)

Made with &nbsp;❤️&nbsp;