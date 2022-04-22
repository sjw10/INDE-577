# K Means Clustering
K Means Clustering is our first example of unsupervised learning. The idea behind k-means clustering is similar to the idea of k nearest neighbors. In K-Means Clustering, the algorithm clusters the data into a set number of groups based on various attributes. The goal of the algorithm is to group the clusters in such a way that the distance between the data points within each cluster is minimized. 
[insert image of centroid]

### Example?

### Implementation
1. Set K number of groups (decide how many groups you want)
2. Initiate K number of random centroids
3. Calculate the distance of all the points to the centroids and using minimum distance to the centroids, split the data into k-groups
4. Average the locations of each group of points to find the new centroids
5. Repeat steps 3-4 until a minimum is achieved

### Potential Issues
If there are too many attributes, there end up being too many dimensions and the data can be extremely far apart, leading to skewed results. In order to combat this, we will implement dimensionality reduction in the subsequent modules to combat this issue.
