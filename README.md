# Unsupervised Machine Learning – Clustering on the Iris Dataset

This project applies **unsupervised learning techniques** to the famous **Iris dataset** to uncover natural groupings of flower species without using their labeled classes during training.

---


## Technologies Used

- **Python**
- **Pandas, NumPy, Matplotlib, Seaborn** – Data analysis and visualization
- **Scikit-learn** – Clustering models, PCA
- **Scipy** – Hierarchical clustering and dendrograms

---

## Dataset Overview

- **Dataset**: [Iris Dataset](https://archive.ics.uci.edu/ml/datasets/iris)
- **Samples**: 150 flower samples
- **Features**:
  - Sepal Length
  - Sepal Width
  - Petal Length
  - Petal Width
- **Classes (for validation only)**:
  - *Iris setosa*
  - *Iris versicolor*
  - *Iris virginica*

> Class labels were excluded during training and only used for post-clustering validation.

---

## Data Exploration & Preprocessing

- Verified **no missing values** or outliers
- Standardized all **numerical features**
- Applied **PCA (Principal Component Analysis)** to reduce dimensionality to 2D for visualization
- Encoded species labels for evaluation purposes only

---

## Clustering Models Trained

| Model               | Details |
|--------------------|---------|
| **K-Means**         | ✅ Optimal **K=3** via Elbow method; clusters clearly matched true species |
| **Hierarchical**    | Agglomerative clustering with Ward’s linkage; good cluster separation |
| **DBSCAN**          | Detected density-based groups; more sensitive to `eps` and `min_samples` |

---

## Final Model Recommendation

** K-Means Clustering (K=3)**

- Best overall clustering performance
- Simple, interpretable, and easy to visualize
- Clusters aligned strongly with actual species:
  - **Cluster 1** → *Iris setosa*
  - **Cluster 2** → *Iris versicolor*
  - **Cluster 3** → *Iris virginica*

---

## Visualizations

- PCA Scatter Plot with Cluster Labels
- Elbow Plot for determining optimal `K`
- Dendrogram for Hierarchical Clustering

> All models visualized in 2D PCA space for interpretability.

---

## Key Insights

- *Iris setosa* is clearly separable from other species
- *Versicolor* and *virginica* show some overlap but are distinguishable
- Clustering techniques can reveal natural structure in unlabeled data



