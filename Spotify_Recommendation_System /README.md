
# **Personalized Music Recommender Systems**

This project explores the construction of recommender systems to personalize music suggestions based on **popularity**, **content**, and **user preferences**. Using various recommendation methods and exploratory data analysis (EDA), we aim to enhance the listening experience and provide tailored playlists for users.

---

## **Business Objective**
The primary objective of this project is to construct effective recommender systems to:
1. Understand traits of popular music through clustering.
2. Generate recommendations for songs and playlists using popularity-based, content-based, and hybrid methods.
3. Evaluate the effectiveness of these methods through experimentation and user feedback.

---

## **Data Sources**
The datasets used in this project include:
1. **Spotify Top 10,000 Songs (1960–2023)**:
   - Track information and audio features (9,999 rows, 35 columns).
   - [Source](https://www.kaggle.com/datasets/joebeachcapital/top-10000-spotify-songs-1960-now/data)
2. **Spotify Playlist Data**:
   - User playlists for artist preference analysis (12,891,680 rows, 4 columns).
   - [Source](https://www.kaggle.com/datasets/andrewmvd/spotify-playlists)
3. **Spotify API**:
   - Personalized playlists for testing recommendations:
     - [Cathy’s Playlist](https://open.spotify.com/playlist/4mDJRCphx1MUd4Dfejj6tj) (16 songs).
     - [Judy’s Playlist](https://open.spotify.com/playlist/32nyghbn3sIw168FA7VKFT) (17 songs).

---

## **Methodology**
### **1. Exploratory Data Analysis (EDA)**
- Identified correlations between features (e.g., Energy, Danceability, Loudness).
- Refined artist genres into 25 main categories for better analysis.
- Analyzed historical trends, such as the rise in explicit tracks and the decline of acousticness.

### **2. Recommendation Methods**
1. **Clustering (PCA + KMeans)**:
   - Applied clustering techniques to group songs based on audio features.
   - Used PCA for dimensionality reduction and the elbow method to set k=6.
2. **Popularity-Based Recommendation**:
   - Recommended songs based on their popularity and global trends.
3. **Content-Based Recommendation**:
   - Recommended songs and playlists by analyzing track features (e.g., Acousticness, Danceability).
4. **Hybrid Recommendation**:
   - Combined popularity, content, and user preferences for a personalized experience.

### **3. Experimentation**
- Evaluated recommendations using manual ratings:
  - Content-Based Model: 8.5/10 (Judy), 9/10 (Cathy).
  - Hybrid Model: 9/10 (both playlists).

---

## **Files**
- **[EDA.ipynb](EDA.ipynb)**: Notebook containing exploratory data analysis.
- **[model.ipynb](model.ipynb)**: Notebook implementing recommendation methods.

---

## **Results and Insights**
- Popular music clusters showed high Loudness, Energy, and Danceability with low Acousticness and Speechiness.
- Hybrid recommendations effectively blended popularity and user-specific preferences, scoring higher in user ratings.

---

## **Recommendations**
1. **Interactive User Interface**:
   - Develop a web app to gather user preferences for better personalization.
2. **Expanded Data Sources**:
   - Include newer songs and user playlist data for a broader analysis.
3. **Testing Metrics**:
   - Implement metrics to fine-tune and improve model performance.


---
## Contributors
-Cathy (Yidan) Wang
-Kexian (Kay) WU
-Judy (Zhiyi) Zhu

---

## **References**
- [Spotify Top 10,000 Songs (1960–2023)](https://www.kaggle.com/datasets/joebeachcapital/top-10000-spotify-songs-1960-now/data)
- [Spotify Playlist Dataset](https://www.kaggle.com/datasets/andrewmvd/spotify-playlists)
- [DamVibes: 25 Types of Music Genres](https://www.damvibes.com/music-theory/25-types-of-music-genres)
