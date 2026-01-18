# 🎬 Movie-Recommender-System

## 📌 Project Overview

This project implements a **Movie Recommender System** that suggests relevant movies based on a user’s input movie selection. It leverages text-based similarity techniques using movie metadata to compute and rank recommendations, helping users discover films similar to those they know and enjoy.

-------------------------------------------------------------------------------------------

## 🚀 Features

  - Takes a **movie title** as input from the user

  - Computes similarity between movies using vectorization techniques

  - Recommends a list of top similar movies

  - Deployed as an interactive web app using **Flask** (app.py)

  - Backend logic implemented in Python with machine learning techniques

-------------------------------------------------------------------------------------------

## 🧠 How It Works

1. **Data Preparation:** Movie metadata (titles, genres, etc.) is cleaned and combined into text features.

2. **Feature Encoding:** Movie metadata is transformed into numerical vectors using TF-IDF and related techniques to capture semantic similarity.

3. **Similarity Computation:** Cosine similarity is computed between movie vectors to measure closeness.

4. **Recommendation:** The top N most similar movies are returned for a user-selected movie.

5. **Deployment:** A simple Flask application hosts the recommendation logic and UI.

-------------------------------------------------------------------------------------------

## 📁 Repository Structure

```
movie-recommender-system/
│
├── Movie_Recommender_System.ipynb     # Core model development & EDA
├── app.py                             # Flask web app for recommendations
├── movies.pkl                         # Preprocessed movie dataset (pickle format)
├── similarity.pkl                     # Precomputed similarity matrix (pickle format)
├── requirements.txt                   # Dependencies
└── README.md                          # Project overview (this file)
```

⚠️ Due to GitHub size limits, download similarity.pkl here:
👉 [Download Link](https://drive.google.com/file/d/1ivssogVryFOXAVMQfKzp9n-iOfYy1XjA/view?usp=sharing)

-------------------------------------------------------------------------------------------

## 🛠️ Tools & Technologies

| Area                   | Technologies                |
| ---------------------- | --------------------------- |
| Programming            | Python                      |
| Data Manipulation      | pandas, numpy               |
| Feature Engineering    | sklearn (TF-IDF vectorizer) |
| Similarity Computation | cosine similarity           |
| Visualization          | seaborn, matplotlib         |
| Deployment             | Flask (app.py)              |
| Notebook Environment   | Jupyter Notebook            |

-------------------------------------------------------------------------------------------

## 🖥️ Demo / How to Use

**Run locally**

1. Clone the repository
   - git clone https://github.com/Prashant2355/movie-recommender-system
   - cd movie-recommender-system
     
2. Install dependencies
   - pip install -r requirements.txt

3. Start the Flask app

   - python app.py

4. Visit:

   - http://127.0.0.1:5000

5. Enter a movie title and get recommendations!

-------------------------------------------------------------------------------------------

## 📊 Key Insights

  - Movie recommendations are based on **content similarity** using text features — **titles, keywords, genres**, etc.

  - The system ranks movies based on **cosine similarity** scores.

  - Pre-computing the similarity matrix allows **fast** lookup at runtime.

  - You can easily extend this to larger datasets or hybrid techniques (collaborative filtering, deep learning, etc.).
