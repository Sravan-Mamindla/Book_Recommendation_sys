# Book Recommendation System

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![NLP](https://img.shields.io/badge/NLP-NLTK%2BScikit--learn-green)
![ML](https://img.shields.io/badge/ML-Cosine%20Similarity-orange)

A content-based recommendation system that suggests similar books using Natural Language Processing (NLP) techniques.

## 📌 Features
- Text preprocessing pipeline for book descriptions
- TF-IDF vectorization with bigrams
- Cosine similarity-based recommendations
- Image display of recommended books
- Genre-specific filtering

## 🛠️ Installation
pip install -r requirements.txt

## 📌 Key Technical Components

### 1. **NLP Preprocessing**
- **ASCII Character Filtering**: Removes non-ASCII characters to ensure clean text input.
- **Stopword Removal**: Uses NLTK's stopwords corpus to eliminate common words that add little meaning.
- **Text Normalization**: Converts text to lowercase and removes punctuation for consistency.
- **HTML Tag Removal**: Strips HTML tags from descriptions using regex.

### 2. **Feature Engineering**
- **Bigram TF-IDF Vectorization**: Converts text into numerical features using Term Frequency-Inverse Document Frequency (TF-IDF) with bigrams to capture word pairs.
- **Cosine Similarity Matrix**: Computes similarity scores between book descriptions to find the most relevant matches.

### 3. **Content Filtering**
- **Genre-Based Filtering**: Filters books by genre before applying similarity measures for more relevant recommendations.
- **Similarity Score Ranking**: Ranks books based on cosine similarity scores and returns the top 5 recommendations.

### 4. **Visualization**
- **Image Display**: Fetches and displays book cover images from URLs using `requests` and `PIL` (Python Imaging Library).
- **Matplotlib Integration**: Renders images in a clean format for easy visualization.
