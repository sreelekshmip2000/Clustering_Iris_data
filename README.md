# Clustering_Iris_data

# Iris Dataset Clustering Project

This project applies unsupervised learning techniques to cluster the Iris dataset using **KMeans** and **Hierarchical Clustering**. The goal is to explore natural groupings within the dataset without using the species labels.

## Objectives
- Load and preprocess the Iris dataset.
- Implement two clustering algorithms:
  - **KMeans Clustering**
  - **Hierarchical Clustering**
- Visualize the clusters using scatter plots and dendrograms.
- Compare how both clustering algorithms group the data.

##  Techniques Used
- Standardization using `StandardScaler`
- KMeans Clustering (`sklearn`)
- Hierarchical Clustering (`scipy`)
- Dendrogram visualization
- Scatter plot visualization of clusters


**1. Loading & Preprocessing**

The Iris dataset was loaded using load_iris() from scikit-learn.
Since clustering is unsupervised, the species column was removed.
StandardScaler was applied to normalize features because clustering algorithms are sensitive to different feature scales.

**2. KMeans Clustering**

How it Works:

Chooses k cluster centroids

Assigns each point to the nearest centroid

Recomputes centroids until convergence

Why Suitable for Iris Dataset:

Iris contains 3 natural groups

Features are numeric and continuous

KMeans works well with compact clusters

**3. Hierarchical Clustering**

How it Works:

Agglomerative (bottom-up) approach

Each data point starts as its own cluster

Clusters merge based on minimum distance

Visual output is a dendrogram

Why Suitable for Iris Dataset:

Data size is small

Good for understanding grouping tendencies

Dendrogram shows natural cluster boundaries

**4. Visualization**

KMeans clusters were plotted using a scatter plot.

Hierarchical clusters visualized using a dendrogram + scatter plot.

Both methods successfully separate Iris-setosa clearly.
