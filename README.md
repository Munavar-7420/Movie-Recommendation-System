<div align="center">

# 🎬 Movie Recommendation System

### Building Personalized Movie Recommendations Using NLP and Machine Learning

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![NLP](https://img.shields.io/badge/NLP-Natural_Language_Processing-blue?style=for-the-badge)
![Machine Learning](https://img.shields.io/badge/Machine_Learning-102230?style=for-the-badge)

</div>

---

## 📌 Project Overview

This project develops a Content-Based Movie Recommendation System using Natural Language Processing (NLP) and Machine Learning techniques.

The system recommends movies based on movie metadata such as genres, keywords, cast members, crew information, and movie descriptions. Similar movies are identified using cosine similarity on text-based features.

The objective is to provide personalized movie recommendations by analyzing movie characteristics and content rather than relying solely on user ratings.

---

## 🎯 Objectives

✔ Build a Content-Based Recommendation Engine

✔ Process and analyze movie metadata

✔ Perform Natural Language Processing (NLP)

✔ Extract meaningful movie features

✔ Calculate movie similarity using Cosine Similarity

✔ Recommend movies based on user preferences

✔ Evaluate recommendation quality

---

## 🧰 Tools & Technologies

<p align="center">

<a href="https://www.python.org/">
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width="50" height="50"/>
</a>

<a href="https://pandas.pydata.org/">
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" width="50" height="50"/>
</a>

<a href="https://numpy.org/">
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" width="50" height="50"/>
</a>

<a href="https://scikit-learn.org/">
<img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" width="50" height="50"/>
</a>

<a href="https://jupyter.org/">
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jupyter/jupyter-original.svg" width="50" height="50"/>
</a>

</p>

---

## 📂 Dataset

**Dataset:** The Movies Dataset

**Source:** https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset

### Dataset Files

#### Credits.csv

- Cast
- Crew
- ID

#### Keywords.csv

- ID
- Keywords

#### Movies_Metadata.csv

- Title
- Genres
- Overview
- Popularity
- Runtime
- Revenue
- Release Date
- Vote Average
- Vote Count
- Production Companies
- Original Language

#### Ratings.csv

- User ID
- Movie ID
- Rating
- Timestamp

#### Links.csv

- Movie ID
- IMDb ID
- TMDB ID

---

## 📊 Dataset Summary

- 45,000+ Movies
- 26 Million+ Ratings
- Multiple Metadata Sources
- User Rating Information
- Movie Keywords and Genres
- Cast and Crew Information

---

## 🔄 Project Workflow

```text
Movie Dataset
      │
      ▼
Data Cleaning
      │
      ▼
Merge Metadata Files
      │
      ▼
Feature Extraction
      │
      ▼
Text Preprocessing (NLP)
      │
      ▼
TF-IDF Vectorization
      │
      ▼
Cosine Similarity Matrix
      │
      ▼
Recommendation Engine
      │
      ▼
Movie Recommendations
```

---

## 🧹 Data Preprocessing

The following preprocessing steps were performed:

- Missing Value Treatment
- Duplicate Removal
- Metadata Integration
- Genre Extraction
- Cast Extraction
- Crew Extraction
- Keyword Processing
- Text Normalization

---

## 🤖 Recommendation Techniques

### Content-Based Filtering

Movies are recommended based on:

- Genres
- Keywords
- Cast
- Director
- Overview
- Movie Tags

### Cosine Similarity

Measures similarity between movie feature vectors and identifies the most relevant recommendations.

### TF-IDF Vectorization

Converts textual movie information into numerical feature vectors for similarity calculations.

---

## 📊 Feature Engineering

Combined movie metadata into a single feature set including:

- Genres
- Keywords
- Cast Members
- Directors
- Movie Overview

Example:

```text
Action Adventure Sci-Fi ChristopherNolan
LeonardoDiCaprio Space Dream Technology
```

---

## 📈 Recommendation Process

### User Input

```text
Movie: Interstellar
```

### System Output

```text
Recommended Movies:

1. Inception
2. The Martian
3. Gravity
4. Arrival
5. Contact
```

---

## 📷 Project Results

### Recommendation Dashboard

<img width="1536" height="1024" alt="Movie Recommendation System" src="https://github.com/user-attachments/assets/26435fda-d7f3-4dfd-ae15-c73e5570a321" />

### Similarity Matrix Visualization

<img width="1536" height="1024" alt="Movie Similarity Matrix" src="https://github.com/user-attachments/assets/36ffa606-b5e5-4dac-9a3c-6329e6663810" />

### Top Recommended Movies

<img width="1693" height="929" alt="Top Recommended Movies" src="https://github.com/user-attachments/assets/6be76055-a69f-49c4-b2b8-0a784826dcd5" />

### Movie Metadata Analysis

<img width="1693" height="929" alt="Movie Metadata Analysis" src="https://github.com/user-attachments/assets/e6134757-8786-463c-951c-36fe42c1406b" />

---

## 📊 Model Evaluation

Evaluation Metrics:

- Cosine Similarity Score
- Recommendation Relevance
- Precision@K
- User Satisfaction Testing

---

## 💡 Key Insights

- Movie genres significantly influence recommendation quality.
- Cast and director information improve recommendation relevance.
- TF-IDF effectively captures movie content characteristics.
- Content-based filtering performs well for cold-start recommendations.
- Combining metadata sources improves recommendation accuracy.

---

## 📁 Repository Structure

```text
Movie-Recommendation-System/
│
├── Data/
│   ├── credits.csv
│   ├── keywords.csv
│   ├── links.csv
│   ├── links_small.csv
│   ├── movies_metadata.csv
│   ├── ratings.csv
│   └── ratings_small.csv
│
├── Notebook/
│   └── Movie_Recommendation_System.ipynb
│
├── Model/
│   ├── similarity.pkl
│   └── movies.pkl
│
├── Pics/
│   ├── recommendation-dashboard.png
│   ├── similarity-matrix.png
│   ├── recommendations.png
│   └── metadata-analysis.png
│
├── README.md
├── LICENSE
├── requirements.txt
└── .gitignore
```

---

## 🚀 Future Improvements

- Collaborative Filtering
- Hybrid Recommendation System
- Deep Learning Recommendations
- User Profile-Based Recommendations
- Streamlit Web Application
- Real-Time Movie Suggestions

---

## 👨‍💻 Author

**Munavar Patter**

Aspiring Data Scientist

Python • Pandas • NLP • Scikit-Learn • Machine Learning • SQL
