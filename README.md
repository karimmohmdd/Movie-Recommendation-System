
# 🎬 Movie Recommender System

## 📌 Project Overview
This project implements a **Content-Based Movie Recommender System** that recommends movies similar to a movie liked by the user.  
In addition to recommendations, the system performs **Sentiment Analysis** on user reviews to analyze audience opinions.

The project combines **API integration**, **web scraping**, **data preprocessing**, and **machine learning** techniques to simulate a simplified Netflix-style recommendation engine.

---

## 🧠 Recommendation Methodology
- **Content-Based Filtering**
- Movies are recommended based on similarity in:
  - Genre
  - Runtime
  - Rating
  - Overview
  - Other metadata
- The system focuses on movie features rather than user-to-user interactions.

---

## 🌐 Data Sources

### 1️⃣ TMDB API
Movie metadata is fetched using **The Movie Database (TMDB) API** by passing the **IMDB ID** of each movie.

**Fetched details include:**
- Movie title
- Genres
- Runtime
- Rating
- Poster
- Release year
- Overview

📎 TMDB API Documentation:  
https://www.themoviedb.org/documentation/api

---

### 2️⃣ IMDB Web Scraping
- User reviews are scraped from **IMDB**
- **BeautifulSoup4** is used for extracting reviews from movie pages
- These reviews are later used for sentiment analysis

---

## 📊 Data Preprocessing
- Datasets were collected from **multiple years**
- Data was available in **different formats and structures**
- A preprocessing pipeline was applied to:
  - Clean missing and inconsistent values
  - Standardize column names
  - Normalize features
  - Convert all datasets into a **unified format**

This ensures compatibility across all movies in the recommender system.

---

## 😊 Sentiment Analysis
- Sentiment analysis is performed on IMDB user reviews
- **Naive Bayes Classifier** is used
- Reviews are classified into:
  - Positive
  - Negative
- Sentiment results provide additional insights into movie popularity and user perception

---

## 🛠 Technologies & Tools
- **Python**
- **TMDB API**
- **Web Scraping**
  - BeautifulSoup4
- **Machine Learning**
  - Naive Bayes
- **Data Processing**
  - Pandas
  - NumPy
- **Natural Language Processing (NLP)**

---

## 🚀 Features
- Real-time movie data fetching using TMDB API
- IMDB review scraping
- Sentiment analysis on user reviews
- Content-based movie recommendations
- Handles datasets from different years and formats

---

## 📌 Conclusion
This project demonstrates a full pipeline for building a recommender system using real-world data.  
It integrates **data processing**, **NLP**, **machine learning**, and **API usage** to deliver meaningful movie recommendations and sentiment insights.

---
