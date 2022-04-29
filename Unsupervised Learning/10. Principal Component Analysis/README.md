# Principal Component Analysis
As mentioned in the previous K-Means Clustering module, sometimes there can be too many attributes for data, leading to too many dimensions that are too far spaced apart, leading to skewed results. Principal Component Analysis is one way to complete dimensionality reduction. The idea behind Principal Component Analysis is to find the dimensions that lead to the most variance and plot the data onto these dimensions. Thus, the data tends to be separated into distinct categories rather than overlapping. 

<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.analyticsvidhya.com%2Fwp-content%2Fuploads%2F2016%2F03%2F1-1.png&f=1&nofb=1" width=80% height=80%>

### Implementation
In order to compare the variances between the data, we must first standardize the data, or in other words, center and scale the data. If we do not complete this step, we could have attributes that have high variances simply because their numbers are bigger. This would lead to incorrect reduction of dimensions. We standardize the data by calculating the z-scores for each data point. After standardizing the data, we need to compute the covariance or correlation matrix in order to find the variances of the various attributes. Then, using the SVD of this matrix, we can see which attributes are most important (using the highest eigenvalues). 

With each eigenvalue we can also find the associated eigenvector (called a principal component), and project the data onto these principal components. Projecting a matrix onto a vector thus reduces the dimension and allows us to complete dimensionality reduction!

# Task
In this module, I will perform Principal Component Analysis on both the red and white wine quality datasets to perform dimensionality reduction. I will then perform random forests and bagging on the reduced dataset and see how the machine performs.
