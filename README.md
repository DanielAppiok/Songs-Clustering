# Music_Clustering

# Spotify Music Clustering Project

This project applies unsupervised machine learning to segment over **580,000 Spotify tracks (1921–2020)** into meaningful clusters based on their audio features. The main goal is to discover natural groupings in music using KMeans clustering and explore characteristics of each cluster.


## Objective

To group songs with similar audio characteristics using unsupervised learning (KMeans), and analyze the resulting music clusters to uncover insights into genre, mood, and style.

---

## Preprocessing Steps

1. Removed unnecessary columns like `id`, `name`, `release_date`, etc.
2. Scaled numeric features using `StandardScaler`.
3. Performed basic EDA to understand feature distributions and ranges.

---

## Clustering Approach

- **Algorithm Used**: KMeans
- **Optimal K**: Determined using Elbow Method and Silhouette Score
- **Number of Clusters**: 6

---

## 📌 Cluster Summary

| Cluster | Danceability | Energy | Loudness | Speechiness | Acousticness | Instrumentalness | Liveness | Valence | Tempo |
|---------|--------------|--------|----------|-------------|--------------|------------------|----------|---------|-------|
| 0       | 0.50         | 0.74   | -6.91    | 0.07        | 0.15         | 0.09             | 0.18     | 0.48    | 140.35 |
| 1       | 0.70         | 0.66   | -8.05    | 0.08        | 0.30         | 0.04             | 0.16     | 0.76    | 114.72 |
| 2       | 0.67         | 0.40   | -15.50   | 0.87        | 0.64         | 0.00             | 0.38     | 0.56    | 102.01 |
| 3       | 0.49         | 0.31   | -12.76   | 0.05        | 0.74         | 0.02             | 0.17     | 0.41    | 110.69 |
| 4       | 0.51         | 0.66   | -8.87    | 0.10        | 0.39         | 0.08             | 0.72     | 0.56    | 120.26 |
| 5       | 0.42         | 0.25   | -17.39   | 0.06        | 0.84         | 0.81             | 0.17     | 0.38    | 107.46 |




## Key Learnings

- KMeans effectively groups songs based on their audio features.
- Certain clusters represent **high-energy dance tracks**, while others contain **acoustic or instrumental-heavy songs**.
- Silhouette Score helped evaluate the compactness and separation of clusters.


## Next Steps

- Add genre tags or mood labels using metadata for deeper analysis.
- Explore other clustering methods (e.g., DBSCAN, GMM) for better separation.
- Build a song recommendation engine based on cluster similarity.


