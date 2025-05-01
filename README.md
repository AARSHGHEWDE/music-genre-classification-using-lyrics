# 🎵 Lyrics-Based Music Genre Classification

This project investigates the potential of using **song lyrics** as a standalone feature for classifying music genres. While traditional classification approaches focus on audio-based signals like tempo, timbre, and rhythm, this work emphasizes the **linguistic and thematic content** embedded in lyrics to identify a song's genre.

---

## 🎯 Problem Context

In the world of digital music, genre classification is a foundational task that powers streaming algorithms, music discovery tools, and playlist generation. Most solutions rely on complex audio signal processing. However, **lyrics—rich in emotion, culture, and narrative—offer genre-specific cues** often overlooked.

For example:
- **Country** lyrics often explore rural life and heartbreak  
- **Rap** lyrics reflect urban struggle, identity, and social commentary  
- **Pop** lyrics tend to emphasize relationships and emotional highs/lows

This project leverages these patterns to build a **purely text-based genre prediction pipeline**—ideal for use cases where audio is unavailable or impractical to process.

---

## 🔍 Project Breakdown

### 🧪 Baseline Modeling

The initial phase uses classical models trained on TF-IDF-transformed lyrics to set a benchmark:

- **Logistic Regression**
- **Random Forest**
- **XGBoost**

Each model learns from lyrical data alone to predict one of several genres. Despite their simplicity, these classifiers proved effective and interpretable, providing a strong baseline for text-based classification.

---

### 🧠 Naive Bayes + Streamlit App

We also implemented a **Multinomial Naive Bayes classifier** with custom NLP preprocessing:
- Tokenization, lemmatization, and stopword removal using NLTK
- TF-IDF vectorization
- Deployed via a **Streamlit web interface** for real-time lyric-based predictions

The model was lightweight, fast, and easy to interpret—making it ideal for deployment scenarios.

---

### ⚙️ Fine-Tuning & Optimization

To push performance further, ensemble models were fine-tuned using hyperparameter optimization:

- **Random Forest** and **XGBoost** were tuned for:
  - `max_depth`, `min_samples_split`, `subsample`, `colsample_bytree`, and more
- This demonstrated that classical ML models—when tuned well—can rival more complex neural approaches.

---

### 📊 Evaluation & Visualization

Comprehensive visualizations were created to analyze and interpret model behavior:

- Genre distribution in the dataset
- Confusion matrices
- Accuracy, precision, recall, and F1 scores
- Bar charts comparing model performance
- Feature importance insights

These tools help assess where lyrical models succeed—and where they struggle (e.g., genres with overlapping vocabulary).

---

## 🛠️ Tools and Technologies

- **Python**
- **Scikit-learn**
- **XGBoost**
- **NLTK**
- **Pandas, NumPy**
- **Matplotlib & Seaborn**
- **Jupyter Notebooks**
- **Streamlit**

---

## 🚀 Outcome

This project shows that **lyrics alone can be powerful predictors of genre**, especially when combined with careful preprocessing and classical ML techniques. It also highlights the practicality of text-only pipelines when audio features are inaccessible.

