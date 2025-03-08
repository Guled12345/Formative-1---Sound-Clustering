# Formative-1---Sound-Clustering

## what is about ?
This assignment explores clustering techniques for unlabeled sound data using **Mel Spectrogram** features, dimensionality reduction (PCA, t-SNE), and clustering algorithms (K-Means, DBSCAN). The goal is to identify meaningful clusters and evaluate their performance.

##  Concepts
### Feature Extraction
- Extracted **Mel Spectrogram** features using `librosa` to represent sound data.

### Dimensionality Reduction
- High-dimensional features made direct clustering challenging.
- **Principal Component Analysis (PCA):** Reduced dimensionality while retaining important variance.
- **t-Distributed Stochastic Neighbor Embedding (t-SNE):** Provided better visualization and improved cluster separation.

### Clustering Techniques
- **K-Means Clustering:** Assigned data points into clusters based on similarity, using the **Elbow Method** to determine optimal k.
- **DBSCAN (Density-Based Spatial Clustering):** Identified clusters based on density but struggled with parameter sensitivity.


## Steps in the Notebook
1. **Load and Preprocess Data:** Standardized features for consistency.
2. **Apply Dimensionality Reduction:** Used PCA and t-SNE for visualization.
3. **Perform Clustering:** Applied K-Means and DBSCAN to group sound features.
4. **Evaluate Results:** Used performance metrics and visualizations to analyze cluster quality.

## Results
- **K-Means:**
  - **Silhouette Score:** 0.7005
  - **Davies-Bouldin Index:** 1.0313 (good separation)
- **DBSCAN:**
  - **Silhouette Score:** -0.0305
  - **Davies-Bouldin Index:** 1.8554 (poor performance)
- **Visualization:** t-SNE provided better cluster separability than PCA.


## Conclusion
Dimensionality reduction (PCA, t-SNE) significantly improved interpretability and clustering efficiency. **K-Means performed well**, while **DBSCAN was less effective** due to the dataset's characteristics. This highlights the importance of choosing the right clustering method based on data distribution.
