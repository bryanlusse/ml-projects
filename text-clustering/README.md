<div align="center">

# Text clustering on News Headlines dataset

![badge](https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
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

This folder hosts a projects that performs unsupervised text clustering on a news headlines dataset. The data comes from the [News Category Dataset](https://www.kaggle.com/datasets/rmisra/news-category-dataset), which contains approximately 200k news headlines from the years 2012 to 2018 obtained from [The Huffington Post](https://www.huffingtonpost.com/).

Unsupervised clustering is clustering without using truth labels to optimize your model. This can be helpful when trying to make sense of a lot of data, and gathering information on large groups in the data. Although the dataset *does* have truth labels, I decided not to use them as an added challenge. Other ML projects will make use of truth labels for classification.

## :carpentry_saw: Preprocessing

Preprocessing of the data was done using standard text preprocessing methods: Removing stopwords, lemmatization, removal of punctuation and tokenization.
Afterwards, vectorization was performed using multiple methods:
- Bag of Words
- Term Frequency - Inverse Document Frequency (TF-IDF) 
- Hashing
- Word2Vec

## :chart_with_upwards_trend: Models

Models used for analysis were K-Means and Density-Based Spatial Clustering of Applications with Noise (DBSCAN). Both are implemented in SKLearn and are easy to use.

## :closed_book: Results

K-Means clustering resulted in the best models. For the vectorization method it was not clear what worked best. Multiple methods should be explored in an unsupervised problem.

## :exclamation: Requirements

Found in [requirements.txt](https://github.com/bryanlusse/ml-projects/blob/master/text-clustering/requirements.txt).


## :open_file_folder: Folder Structure

```
.
├── data                                # News dataset
├── assets                              # Images for notebook
├── Text_Clustering.ipynb               # Main notebook
├── iframe_figures                      # Plots of words in clusters
├── outputs                             # Processed data and cluster labels
├── requirements.txt                    # Required packages
└── README.md
```

## :smiley_cat: Author

- [@bryanlusse](https://github.com/bryanlusse)

Made with &nbsp;❤️&nbsp;