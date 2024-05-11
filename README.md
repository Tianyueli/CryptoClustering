# CryptoClustering

# Overview 
- This project demonstrated my ability to use Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.
  
# Model building & Prediction
- Used the the K-means model to cluster the cryptocurrencies for the best value for k on the original scaled data, and predicted the clusters to group the cryptocurrencies using the original scaled DataFrame.

- Created a scatter plot using hvPlot to visualize the two prominent features identified by : the x_axis as "PC1" and the y-axis as "PC2". Additionally, I used the "coin_id" column in the hover_cols parameter to identify the cryptocurrency represented by each data points.


- Next, I used the original scaled DataFrame and performed a PCA(Principal Component Analysis) to optimize the clusters by reducing all the available features to three principal components.
The explained variance was calculated to determine how much information can be attributed to each principal component to identify which of them contain the highest impact to the model.

- Furthermore, I used the PCA data to find the best value for K, which turned out to be the same number(k=4) we identified using original non-compressed data.

- Lastly, I created a K-means model and predicted the clusters to group the cryptocurrencies using the PCA data.
I then plotted a scatter using hvPlot to display the two dominant features cateogrized by coin ID.

# Analysis
- I visually analyzed the cluster analysis results by contrasting the outcome with and without using the optimization techniques. Both elbow curves used to help determine the best quantity of clustering of data showed the ideal number of groupings as 4.

- Both models arrived at recognizing coin IDs "ethlend", "celciusdegreetoken" as outliers

- After visually analyzing the cluster analysis results, here're some obeservations on impact of using fewer features to cluster the data using K-Means:
  - The inertia decreased(shifted down vertically on y_axis);
  - The data points are more compressed and less dispersed
  - In this project, there was nearly no impact to the end result of find the optimal k value
