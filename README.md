<h2>About the Data</h2>
The Iris dataset is a well-known dataset in the field of machine learning. It consists of 150 samples from three species of Iris flowers: Iris setosa, Iris versicolor, and Iris virginica. Each sample has four features: sepal length, sepal width, petal length, and petal width. The dataset also includes the species class for each sample, which is used for validation but excluded from unsupervised learning tasks.
<br>
<br>
<h2>Data Exploration and Cleaning</h2>
Data exploration revealed that the dataset is clean with no missing values. The following preprocessing steps were performed:
<br>
<br>
<ul>
  <li>Standardized numerical features to ensure uniformity.</li>
  <li>Encoded the species class for validation purposes.</li>
  <li>Applied PCA to reduce the dataset to two dimensions for visualization.</li>
</ul>

<h2>Model Training</h2>
Three variations of clustering models were trained on the data set:
<br>
<br>

<b>K-Means Clustering:</b>
<ul>
  <li>The optimal number of clusters (K) was determined using the Elbow method, resulting in K=3.</li>
  <li>The clustering produced clear separations corresponding to the three Iris species.</li>
</ul>

<b>Hierarchical Clustering:</b>
<ul>
  <li>Agglomerative clustering with Ward's linkage was used.</li>
  <li>The resulting clusters also corresponded well to the three species.</li>
</ul>

<b>DBSCAN (Density-Based Spatial Clustering of Applications with Noise):</b>
<ul>
  <li>Parameters epsilon and minimum samples were tuned.</li>
  <li>DBSCAN identified the clusters effectively but was sensitive to parameter changes.</li>
</ul>

 <h2>Model Selection and Recommendation</h2>
Among the three models, K-Means Clustering with K=3 was recommended as the final model. This choice was based on:
<br>
<br>

<ul>
  <li>The clear separation of clusters observed in the visualizations.</li>
  <li>The model's ability to accurately identify the three Iris species.</li>
  <li>The simplicity and interpretability of the K-Means algorithm.</li>
</ul>

<h2>Insights and Key Findings</h2>
The key findings from the clustering analysis include:
<br>
<br>

Cluster 1: Corresponds to Iris setosa, which is distinctly separated from the other species.
<br>
<br>
Cluster 2: Primarily contains Iris versicolor samples.
<br>
<br>
Cluster 3: Primarily contains Iris virginica samples.
<br>
<br>

These insights demonstrate the effectiveness of clustering in identifying natural groupings within the dataset.


 
