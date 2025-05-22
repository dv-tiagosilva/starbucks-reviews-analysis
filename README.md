
# 🧠 Supervised vs Unsupervised Sentiment Analysis 

This project explores the use of **supervised learning** vs **unsupervised learning** to perform **sentiment analysis** on a small dataset of user reviews.

## What this project does (on unsupervised version):
- Preprocesses user reviews
- Generates contextual embeddings
- Applies KMeans clustering to identify sentiment groups (positive/negative) on unsupervised trials
- Clusters visualization (unsupervised)

## What this project does (on supervised version):
- Data cleaning and Preprocesses user reviews
- Classified the sentiment groups (positive/negative/neutral) with the rating from the users reviews
- Uses techniques of undersampling (Random undersampling) and oversampling (SMOTE) for balancing the dataset

## 📊 Dataset
A small set of user reviews from starbucks dataset, avaiable on kaggle: https://www.kaggle.com/datasets/harshalhonde/starbucks-reviews-dataset
 
## Observations to Unsupervised approach
- Initial clustering with basic embeddings was ineffective (Silhouette Score ≈ 0.003)
- After applying SBERT, the clustering improved significantly (Silhouette Score ≈ 0.0659)
- Visual inspection and manual validation confirmed clearer separation of sentiments
- Some reviews remain ambiguous due to neutral language or context complexity

## Observations to Supervised approach
- Great f-1 score achieved!
- I have done some tests and although the f-1 score is pretty impressive, the model is only accurate to identify positive and negative versions, but the neutral group is not well defined.
```

## ⚠️ Disclaimer
This is an **experimental project** designed for exploration and learning purposes. 
