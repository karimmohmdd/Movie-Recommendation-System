# Movie-Recommendation-System
🎬 Building and Deploying a Netflix Recommender System

📌 Overview
This project implements a Content-Based Recommender System that suggests movies similar to a movie liked by the user.
In addition to similarity-based recommendations, the system also performs Sentiment Analysis on user reviews to better understand audience opinions about the movie.

The goal is to simulate a simplified version of a Netflix-style recommendation engine using real-world data sources and machine learning techniques.


🧠 Recommendation Approach

Content-Based Filtering

Recommends movies based on similarity in content such as:

Genre

Runtime

Rating

Overview

Other metadata

The system does not depend on other users’ behavior, but instead focuses on the characteristics of the selected movie.

🌐 Data Sources
1️⃣ TMDB API

Movie details are fetched using The Movie Database (TMDB) API:

Movie title

Genres

Runtime

Rating

Poster

Release year

Other metadata

The TMDB API is accessed using the IMDB ID of each movie.
🔗 TMDB API Documentation:
https://www.themoviedb.org/documentation/api

2️⃣ IMDB Web Scraping

User reviews are collected directly from IMDB using web scraping

BeautifulSoup4 is used to extract reviews from movie pages

These reviews are later used for sentiment analysis

📊 Data Preprocessing

Movie datasets were collected from different years and multiple sources

Data came in different formats and structures

A preprocessing pipeline was applied to:

Clean missing and inconsistent values

Normalize columns and feature names

Convert all datasets into a unified and consistent format

This step ensures that all movies can be processed and compared correctly by the recommender system

😊 Sentiment Analysis

Sentiment analysis is performed on IMDB user reviews

Naive Bayes Classifier is used for classifying reviews into:

Positive

Negative

The sentiment score helps in understanding overall user opinion about a movie and adds more insight to the recommendation process

🛠 Technologies & Tools Used

Python

TMDB API

Web Scraping

BeautifulSoup4

Machine Learning

Naive Bayes (Sentiment Analysis)

Data Processing

Pandas

NumPy

Text Processing

NLP techniques for cleaning and vectorizing reviews

🚀 Features

Fetches real-time movie metadata using TMDB API

Scrapes real user reviews from IMDB

Performs sentiment analysis on reviews

Recommends movies similar to a selected movie

Handles datasets from different years and formats efficiently

📌 Conclusion

This project demonstrates how recommendation systems can be built using content-based filtering, real APIs, web scraping, and machine learning.
It combines data engineering, NLP, and ML concepts into one complete pipeline, making it a practical and educational implementation of a movie recommender system.
