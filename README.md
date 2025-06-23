# 🎬 Netflix Movie Recommendation System


https://github.com/user-attachments/assets/4d13646f-a6fd-4fc1-b7cf-7dadb32d1c1a



A personalized movie recommendation system inspired by Netflix, built using **Machine Learning** and **Data Science** techniques. This project demonstrates my ability to collect, preprocess, and analyze real-world data to generate meaningful movie suggestions for users using **content-based filtering**.

---

## 📌 Project Overview

This system recommends movies based on the content similarity of films. By analyzing metadata like genres, keywords, cast, and crew, it calculates similarity scores using **cosine similarity** and suggests the most similar titles.

---

## 🧠 Methodology

1. **Data Collection & Merging**
   - Combined multiple `.csv` datasets including:
     - `movies.csv`
     - `credits.csv`
     - `keywords.csv`
     - `links.csv`
     - `ratings.csv`

2. **Data Preprocessing**
   - Extracted relevant columns (`title`, `overview`, `genres`, `cast`, `crew`, etc.)
   - Cleaned and normalized text data (e.g., lowercasing, removing spaces, stemming)
   - Parsed JSON-like columns to extract key tokens (actors, directors, keywords)

3. **Feature Engineering**
   - Created a new feature called `tags` by combining important metadata
   - Applied **CountVectorizer** to convert textual data into numerical vectors

4. **Similarity Calculation**
   - Calculated **cosine similarity** between movie vectors
   - Sorted and recommended top 5 similar movies

---

## 🧪 Technologies Used

| Category            | Technologies/Tools                         |
|---------------------|--------------------------------------------|
| Programming         | Python                                     |
| Libraries           | Pandas, NumPy, Scikit-learn, NLTK, Ast     |
| NLP Techniques      | Tokenization, Stemming (Porter Stemmer)   |
| Vectorization       | CountVectorizer (Bag of Words Model)       |
| Similarity Metric   | Cosine Similarity                          |
| Visualization       | Streamlit (optional UI for recommendations)|
| IDE / Environment   | Jupyter Notebook, VS Code                  |

---

## 📁 Dataset

The dataset is built by combining several publicly available `.csv` files provided in the tutorial. The merged dataset was custom-created by:
- Reading raw files
- Cleaning missing values
- Extracting key features (title, genres, cast, etc.)
- Merging `movies` and `credits` data based on `id`

> Final dataset contains approximately **4800+ movies** with rich metadata.

---
