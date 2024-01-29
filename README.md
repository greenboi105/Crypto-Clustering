# Crypto Clustering

In this analysis we want to use unsupervised learning to determine if cryptocurrencies are affected by 24-hour or 7-day price changes.

There are a few major components of the analysis:

1. Determing the best k value using the original scaled DataFrame

    - We use the elbow method to find the best k value.

2. Cluster Cryptocurrencies with K-Means using the original scaled data

    - We cluster the cryptocurrencies with the best value for k.

    - We initialize the K-means model with the best value for k, then fit the K-means model using the original scaled DataFrame.

    - We predict the clusters to group the cryptocurrencies using the original scaled DataFrame.

3. Optimize Clusters with PCA

    - Using the original scaled DataFrame, we perform a PCA and reduce the features to three principal components.

4. Finding the best value for k with the PCA data

    - We use the elbow method on the PCA data to find the best value for k

5. Cluster Cryptocurrencies with K-Means Using the PCA Data

    - We use the steps to cluster the cryptocurrencies for the best value for k on the PCA data
