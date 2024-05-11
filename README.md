# CryptoClustering

# Overview of model building and prediction generation: 
Cluster Cryptocurrencies with K-means Using the Original Scaled Data

- Used the the K-means model to cluster the cryptocurrencies for the best value for k on the original scaled data, and predicted the clusters to group the cryptocurrencies using the original scaled DataFrame.

- Created a scatter plot using hvPlot to visualize the two prominent features identified by : the x_axis as "PC1" and the y-axis as "PC2". Additionally, I used the "coin_id" column in the hover_cols parameter to identify the cryptocurrency represented by each data points.


- Next, I used the original scaled DataFrame and performed a PCA(Principal Component Analysis) to optimize the clusters by reducing all the available features to three principal components.
The explained variance was calculated to determine how much information can be attributed to each principal component to identify which of them contain the highest impact to the model.
