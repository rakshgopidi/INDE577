# K-Means Clustering:
This repository contains an implementation of K-Means clustering algorithm using Python and Scikit-learn library.

**Introduction**
K-Means clustering is an unsupervised machine learning algorithm that is used to partition a dataset into K clusters, where K is a predefined number of clusters. The algorithm works by iteratively assigning data points to the closest centroid and then recomputing the centroid of each cluster until convergence. The resulting clusters are formed based on the Euclidean distance between the data points and the centroids.

**Dataset**
The dataset used in this implementation is the Mall Customer Segmentation Data available on Kaggle. This dataset contains information about customers of a mall, including their age, gender, annual income, and spending score. The objective of the K-Means clustering algorithm is to segment the customers into different groups based on their spending habits.

**Algorithm**
The K-Means algorithm consists of the following steps:

Initialize K centroids randomly
Assign each data point to the closest centroid
Compute the centroid of each cluster
Repeat steps 2 and 3 until convergence (i.e., when the centroids do not change significantly)
To find the optimal number of clusters, the elbow method can be used. In this method, the sum of squared distances between the data points and their assigned centroids is calculated for different values of K, and the optimal value of K is the one where the decrease in the sum of squared distances begins to level off (forming an "elbow" shape).


**Evaluation and Performance**
To evaluate the performance of the K-Means algorithm, the Silhouette Coefficient can be calculated. This coefficient is a measure of how similar an object is to its own cluster compared to other clusters, and ranges from -1 to 1. A higher value indicates that the object is well-matched to its own cluster and poorly-matched to neighboring clusters.

The K-Means algorithm has a few limitations, including sensitivity to the initial random centroids, inability to handle non-spherical clusters, and difficulty in determining the optimal number of clusters.

**Conclusion**
K-Means clustering is a popular unsupervised machine learning algorithm used for clustering data. In this implementation, we used the algorithm to cluster customers of a mall based on their spending habits. The algorithm was evaluated using the Silhouette Coefficient, and its limitations were discussed. Overall, K-Means clustering is a useful tool for exploring and analyzing datasets with unknown structure.
