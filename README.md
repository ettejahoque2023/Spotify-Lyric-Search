# 🎵 Spotify Lyric Search – Song & Artist Identification using NLP

## 📌 Project Overview
Spotify Lyric Search is a beginner-friendly **Machine Learning + NLP project** that identifies the **Song Name, Artist, and Song Link** when given a small snippet of song lyrics.

The system works by converting lyrics into numerical vectors and finding the most similar song from a large dataset using text similarity techniques.

---

## 🎯 Problem Statement
Given a short text snippet from a song’s lyrics, the system predicts:
- 🎵 Song Name  
- 🎤 Artist Name  
- 🔗 Song Link  

---

## 🧠 Solution Approach
Instead of treating this as a classification problem, the project approaches it as a **text similarity / information retrieval problem**.

**Core Idea:**  
If two lyrics are similar in meaning, they will be close to each other in vector space.

---

## 🛠️ Technologies Used
- Python  
- Pandas & NumPy  
- NLTK (Text Preprocessing)  
- Scikit-learn  
- TF-IDF Vectorizer  
- Cosine Similarity  
- Google Colab  

---

## 📂 Dataset
- Source: Kaggle (Spotify / Lyrics Dataset)
- Size: 50,000+ songs
- Important columns used:
  - `song` → Song title  
  - `artist` → Artist name  
  - `text` → Song lyrics  
  - `link` → Lyrics page link  

---

## 🔄 Project Workflow
<img width="351" height="317" alt="image" src="https://github.com/user-attachments/assets/095f8033-9975-46da-a9c0-03dab8f517ec" />

---

## 🧹 Text Preprocessing
Lyrics are cleaned using the following steps:
- Converting text to lowercase
- Removing punctuation and numbers
- Stop-word removal
- Lemmatization

This improves matching accuracy by removing noise from the text.

---

## 🔢 Feature Extraction
- **TF-IDF (Term Frequency – Inverse Document Frequency)** is used
- Converts text data into numerical vectors
- Assigns higher importance to rare and meaningful words

---

## 🤖 Algorithm Used
### ✅ TF-IDF + Cosine Similarity

**Why this algorithm?**
- Works very well for partial lyrics matching
- No heavy model training required
- Efficient and fast for large datasets
- Easy to understand and explain in interviews

---

## 🧪 Sample Prediction
<img width="1048" height="261" alt="Screenshot 2025-12-30 205040" src="https://github.com/user-attachments/assets/ef36b22c-786e-4d84-8b0f-67cb922ecbe9" />

---
## 📁 Project Structure
Spotify-Lyric-Search/
│
├── spotify_lyric_search.ipynb
├── README.md
├── requirements.txt

---

## ▶️ How to Run the Project
1. Open the notebook in **Google Colab**
2. Upload the dataset CSV file
3. Run all cells sequentially
4. Use the function below to test:
```python
predict_song("your lyrics snippet here")
