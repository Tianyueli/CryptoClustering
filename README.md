# CryptoClustering

# Overview 
- This project demonstrated my ability to use Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.
  
# Model building & Prediction
- I used the K-means model to cluster the cryptocurrencies for the best value for k on the original scaled data. I predicted the clusters would group the cryptocurrencies using the original scaled data frame.

I created a scatter plot using hvPlot to visualize the two prominent features identified by the x_axis as "PC1" and the y-axis as "PC2." I also used the "coin_id" column in the hover_cols parameter to determine the cryptocurrency represented by each data point.


- Next, I used the original scaled DataFrame and performed a PCA(Principal Component Analysis) to optimize the clusters by reducing all the available features to three principal components.
I calculated the explained variance to determine how much information is attributed to each principal component and to identify which has the highest impact on the model.

- I used the PCA data to find the best value for K, which was the same number(k=4) we identified using original non-compressed data.

- I created a K-means model and predicted the clusters to group the cryptocurrencies using the PCA data.
I then plotted a scatter using hvPlot to display the two dominant features categorized by coin ID.

# Analysis
- I visually analyzed the cluster analysis results by contrasting the outcome with and without using the optimization techniques. Both elbow curves used to help determine the best quantity of data clustering showed the ideal number of groupings as 4.

- Both models arrived at recognizing coin IDs "ethlend" and "celciusdegreetoken" as outliers

- After visually analyzing the cluster analysis results, here are some observations on impact of using fewer features to cluster the data using K-Means:
  - The inertia decreased(shifted down vertically on y_axis);
  - The data points are more compressed and less dispersed
  - In this project, there was nearly no impact on the end result of finding the optimal k-value
