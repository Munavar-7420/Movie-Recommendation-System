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

✔ Clean and merge multi-table movie metadata 
✔ Parse nested JSON strings for genres, cast, crew, and keywords  
✔ Normalize text tags and apply **TF-IDF Vectorization**  
✔ Compute a **Cosine Similarity** matrix to rank similar films  
✔ Solve the cold-start recommendation problem for new or unrated titles  

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

**Source:** [Kaggle Movies Dataset](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset)

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
Movie Metadata Files
        │
        ▼
Data Cleaning & Metadata Merging
        │
        ▼
JSON Parsing (Genres, Keywords, Cast, Director)
        │
        ▼
Text Normalization & Tag Soup Creation
        │
        ▼
TF-IDF Vectorization
        │
        ▼
Cosine Similarity Matrix
        │
        ▼
Top-N Movie Recommendations
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

## 📊 Feature Engineering & Example Output

Combined cleaned metadata attributes into a unified text representation (e.g., `Action Adventure Sci-Fi ChristopherNolan LeonardoDiCaprio Space Dream Technology`) before vectorizing with TF-IDF.

- **Sample Input:** `Interstellar`
- **Top 5 Recommendations:** `1. Inception` • `2. The Martian` • `3. Gravity` • `4. Arrival` • `5. Contact`

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

- **Metadata Synergy:** Combining director, top-billed cast, and thematic keywords alongside genres produces noticeably tighter recommendations than genre matching alone.
- **Name Tokenization:** Stripping spaces from cast and director names (e.g., `ChristopherNolan`) prevents unrelated matches on common first names.
- **Cold-Start Advantage:** Content-based filtering reliably recommends niche or newly released movies even when user rating history is sparse.

---

## 📁 Repository Structure


```text
Movie-Recommendation-System/
│
├── Data/
│   ├── keywords.csv
│   ├── links.csv
│   ├── links_small.csv
│   ├── movies_metadata.csv.gz
│   └── ratings_small.csv
│
├── Notebook/
│   └── Movie_Recommendation_System.ipynb
│
├── pics/
│   ├── recommendation-dashboard.png
│   ├── similarity-matrix.png
│   ├── recommendations.png
│   └── metadata-analysis.png
│
└── README.md
```

---

## 🚀 Future Improvements

- Hybrid recommendation system combining Collaborative Filtering (SVD) with Content-Based Filtering
- Semantic embeddings using Sentence-BERT / Transformers
- Interactive movie search web app deployed via Streamlit

---

## 👨‍💻 Author

**Munavar Patter**  
M.Sc. Student at SRH University | Former Data Analyst  
Python • Pandas • NLP • Scikit-Learn • Machine Learning • SQL
