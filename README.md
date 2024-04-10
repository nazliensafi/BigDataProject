# Big Data 2024, Group 28 Project Summary

## Project Definition

This project aims to develop a recommender system for suggesting books to users based on their historical ratings. The system seeks to uncover and analyze patterns in movie preferences and provide personalized book recommendations.

## Dataset

Contains 278,858 users (anonymized but with demographic information) providing 1,149,780 ratings (explicit / implicit) about 271,379 books, in the following CSV files:
BX-Book-Ratings.csv
BX-Users.csv
BX_Books.csv
In this project, we use "BX-Book-Ratings.csv" file containing "User-ID", "ISBN", "Book-Rating", delimited by ";" to build the models and "BX_Books.csv" to fetch the titles of the recommended books.
The dataset is available to download at:
(https://www.kaggle.com/datasets/ruchi798/bookcrossing-dataset?resource=download-directory)

## Research Questions

The core questions guiding this project are:

- How can we accurately recommend books to users based on their past interactions?
- What models to use on this large dataset? and how do we compare them?
- How do we test the performance and ensure the quality of the results?

## Model Design and Implementation

We plan to use Collaborative Filtering approach, leveraging matrix factorization techniques to predict user ratings for books they haven't yet read. The primary algorithm used is the ALS (Alternating Least Squares) method in Apache Spark MLlib, chosen for its scalability and effectiveness in handling sparse datasets.
As it is shown to be more efficient in practice, we will explore the possibility of item-item Collaborative Filtering as opposed to user-item CF which Apache Spark uses. Finally, we will evaluate the recommendation model by measuring the root-mean-square error of rating prediction.

### References:

- Mining of massive datasets/. Mining of Massive Datasets/Chapter 9 Recommendation Systems. (n.d.). http://www.mmds.org/
- Collaborative filtering. Collaborative Filtering - Spark 2.2.0 Documentation. (n.d.). https://spark.apache.org/docs/2.2.0/ml-collaborative-filtering.html
- Bhatia, R. (2021, February 17). Book-crossing: User review ratings. Kaggle. https://www.kaggle.com/datasets/ruchi798/bookcrossing-dataset?resource=download-directory

### Contributers:

Nazli Ensafi, Korjon Chang-Jones, Anh Tu chau, Cedric Paradis
