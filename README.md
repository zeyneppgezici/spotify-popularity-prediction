# 🎧 Spotify Song Popularity Prediction (Random Forest + SHAP)

This project predicts the **popularity score of Spotify songs** using their audio features and a **Random Forest Regressor** with **SHAP explainability**.

It is designed as a **data analytics & machine learning case study** to showcase:

- Data loading & cleaning  
- Exploratory data analysis (EDA)  
- Feature engineering  
- Regression modeling  
- Model evaluation  
- Model explainability (SHAP)

---

## 📂 Dataset

The dataset contains **~32,000 songs**, each with a variety of audio-related features such as:

- `danceability`
- `energy`
- `loudness`
- `speechiness`
- `acousticness`
- `instrumentalness`
- `liveness`
- `valence`
- `tempo`
- `duration_ms`
- Target: **`track_popularity`**

> The dataset is loaded from `spotify_songs.csv` in the notebook.

---

## 🎯 Business Question

> **Can we predict how popular a song will be based on its audio characteristics?**

In other words, can we build a model that learns patterns from Spotify audio features and outputs a **track popularity score** that is reasonably close to the real-world popularity?

---

## 🧮 Project Workflow

1. **Data Loading**
   - Read the Spotify dataset from `spotify_songs.csv`
   - Inspect the first rows and dataset info

2. **Data Cleaning & Preparation**
   - Handle missing values  
   - Select numeric features for modeling  
   - Standardize / scale features where necessary  
   - Create train–test split for regression

3. **Exploratory Data Analysis (EDA)**
   - Distribution of `track_popularity`
   - Correlation between numerical features
   - Understanding which features are likely to influence popularity

   Example visualizations:

   ```markdown
  ![Feature Importance](images/feature_importance_3.png)
  ![SHAP Summary Plot](images/shap_summary_4.png)


