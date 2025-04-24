# 🎵 Lyrics-Based Music Genre Classification

This project investigates the potential of using **song lyrics as a standalone feature** for classifying music genres. While traditional classification approaches focus on audio-based signals like tempo, timbre, and rhythm, this work emphasizes **linguistic and thematic content** embedded in lyrics to identify a song's genre.

---

## 🎯 Problem Context

In the world of digital music, genre classification is a foundational task that powers streaming algorithms, music discovery tools, and playlist generation. Most solutions rely on complex audio signal processing. However, lyrics—being rich in thematic patterns, cultural references, and emotional tone—hold **valuable genre-specific signals** that are often overlooked.

For instance, **country lyrics** may explore rural life and heartbreak, while **rap lyrics** often reflect urban struggles, self-expression, and social commentary. This project leverages these patterns to build a purely text-based genre prediction pipeline, suitable for scalable classification where audio isn't available or is impractical to process.

---

## 🔍 Project Breakdown

### 🧪 Baseline Modeling
The first phase of this project establishes benchmarks using:
- **Logistic Regression**
- **Random Forest**
- **XGBoost**

Lyrics are converted into numerical form using **TF-IDF vectorization**, and each model is trained to predict one of several possible genres. These models serve as a performance baseline and demonstrate how even simple classifiers can yield useful results from lyrical content alone.

---

### ⚙️ Fine-Tuning & Optimization
To push the performance ceiling higher, ensemble models were **fine-tuned using hyperparameter tuning**:
- **Random Forest** and **XGBoost** were optimized for depth, learning rate, regularization, sampling, and more.
- Parameters like `max_depth`, `subsample`, `colsample_bytree`, and `min_samples_split` were carefully tuned for generalization and robustness.

This phase highlights how tuning classical models can rival more complex solutions with efficient computation.

---

### 📊 Evaluation & Visualization
To understand model behavior and prediction patterns, visualizations were created to show:
- Genre distribution across the dataset
- Confusion matrices and performance metrics (accuracy, precision, recall)
- Feature importance and misclassification trends

These insights help refine the approach and assess where lyrical classification succeeds or fails.

---

## 🛠️ Tools and Technologies

- Python  
- Scikit-learn  
- XGBoost  
- Pandas, NumPy  
- Matplotlib & Seaborn  
- Jupyter Notebooks  
