# News Clustering using Sentence Transformers and Clustering Algorithms

This project tackles the task of **unsupervised clustering of news articles** using **sentence embeddings** from a pretrained transformer model and classic clustering techniques. The primary goal is to group news texts based on semantic similarity, enabling automatic categorization and exploration of textual datasets.

## Objectives

- Extract semantic feature vectors from news data using `all-MiniLM-L6-v2` model from HuggingFace.
- Apply and compare multiple clustering algorithms on the resulting embeddings.
- Evaluate clustering quality using Silhouette Score and Homogeneity Score.
- Visualize high-dimensional embeddings using PCA for intuitive understanding.

## Workflow Overview

1. **Data Preprocessing**:
   - Lowercasing, stop word removal, token normalization.
   - Optional: stemming or lemmatization.

2. **Embedding Extraction**:
   - Used Sentence Transformers (`all-MiniLM-L6-v2`) for high-quality text embeddings.

3. **Clustering Algorithms**:
   - K-Means (with elbow method for optimal K)
   - DBSCAN (density-based)
   - Hierarchical Clustering (agglomerative)
   - Cluster visualizations and comparative analysis included.

4. **Dimensionality Reduction**:
   - PCA used to reduce embeddings to 2D for visualization.

5. **Evaluation Metrics**:
   - Silhouette Score: Measures cohesion vs. separation.
   - Homogeneity Score: Measures if clusters contain only data points which are members of a single class.

## Key Insights

- Sentence-BERT embeddings effectively capture contextual relationships in news data.
- K-Means worked well with well-separated clusters, while DBSCAN better handled noise.
- Dimensionality reduction was crucial for visualization and insight generation.

---

> Course: Artificial Intelligence – Fall 1403  
> University of Tehran | School of Electrical & Computer Engineering