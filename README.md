# Lab 3: Clustering Analysis Using K-Means and K-Medoids Algorithms

**Course:** MSCS-634-B01 — Advanced Big Data and Data Mining  
**Student:** Xhon Pelushi  
**University:** University of the Cumberlands

## Purpose

This lab explores unsupervised clustering on the Wine Dataset using K-Means and
K-Medoids algorithms. Both methods are applied with k=3 and evaluated using
Silhouette Score and Adjusted Rand Index. Results are projected to 2D via PCA
for visual comparison.

## Key Insights

- Both K-Means and K-Medoids produce meaningful clusters that align with the
  true wine classes when the data is standardized.
- K-Means uses computed centroids (geometric means), while K-Medoids uses
  actual data points as cluster representatives, making it more robust to outliers.
- K-Means is computationally faster (O(nk) per iteration) and is the better
  default for clean, spherical clusters.
- K-Medoids is preferable when data contains outliers or when cluster
  representatives must be interpretable real data points.

## Challenges

- The `sklearn_extra` package had a numpy compatibility issue, so K-Medoids
  was implemented manually using pairwise distance matrices.
- PCA was used for visualization but captures only a portion of the total
  variance, so the 2D plots may not perfectly represent the clustering quality
  in the full 13-dimensional space.

## Files

| File | Description |
|------|-------------|
| `Lab3_Clustering_KMeans_KMedoids.ipynb` | Jupyter Notebook with clustering code, metrics, and visualizations |
| `README.md` | This file |
