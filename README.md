
# 🧠 Unsupervised Sentiment Analysis with SBERT and Clustering

This project explores the use of **unsupervised learning** to perform **sentiment analysis** on a small dataset of user reviews, using **sentence embeddings (SBERT)** and **clustering algorithms (KMeans + UMAP)**.

## 🚀 What this project does:
- Preprocesses user reviews
- Generates contextual embeddings using `all-mpnet-base-v2` from SentenceTransformers
- Applies KMeans clustering to identify sentiment groups (positive/negative)
- Visualizes clusters with UMAP
- Detects and ranks ambiguous reviews using distance to cluster centroids

## 📊 Dataset
A small set of user reviews, originally unlabeled, was used to identify potential **positive and negative sentiment clusters** without prior annotations.

## 🔍 Key Techniques Used
- **SBERT embeddings** (`all-mpnet-base-v2`) to capture contextual meaning
- **KMeans** for unsupervised clustering into 2 sentiment-based groups
- **UMAP** for 2D visualization of the clusters
- **Silhouette Score** to evaluate cluster quality
- **Ambiguity Analysis** using distance from cluster centroids

## Observations
- Initial clustering with basic embeddings was ineffective (Silhouette Score ≈ 0.003)
- After applying SBERT, the clustering improved significantly (Silhouette Score ≈ 0.0659)
- Visual inspection and manual validation confirmed clearer separation of sentiments
- Some reviews remain ambiguous due to neutral language or context complexity
```

## ⚠️ Disclaimer
This is an **experimental project** designed for exploration and learning purposes. The model is **unsupervised** and not intended for production-level sentiment classification.
