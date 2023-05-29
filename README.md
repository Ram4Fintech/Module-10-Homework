# Module-10-Homework
# Crypto Clustering:
## Mission:
 To create a portfolio of crypto currencies by analysing their performances over different time periods and after applying different criteria
## Initial steps: 
These initial steps were already provided in the starter code – Import of all the requisite libraries namely, pandas, hvplot, K-means, PCA and StandardScaler from sklearn . Then the csv data file was read as a Pandas DataFrame. The DataFrame was visualised as an hvplot diagram
## Finding the best value for k using original data: 
 Using the elbow method algorithm, I created the k means model, fitted the original scaled data into it and appended the model.inertia to the inertia list. A DataFrame of the elbow data was created using the x and y axis as k and inertia respectively. This DataFrame was further visualised as an hvplot as follows:  
The optimum value of k was visually identified from the above Elbow Curve
## Cluster Cryptos using K-means with original data:  Using the K-means models with 4 clusters and again fitting it with the original scaled data, I used the .predict function to predict the clusters of crypt o currencies. This output was then visualised as a scatter plot as follows: 

## Optimise Clusters with PCA: I created the PCA model and optimised it with 3 components. After viewing this DataFrame, I could conclude that about 88% of the total variance is condensed into the 3 reduced PCA variables. A new DataFrame was created with the 3 PCA variables with coin_id as the index.
*Finding the best value of k with PCA data: A k-means model was again created with the PCA data and the resultant DataFrame was visually represented in the form of an Elbow curve with the same x and y axis as was done earlier. The hvplot line looks like this:
 ![Decorative image.](Image/Elbow.png)



## Cluster Cryptocurrencies with K-means Using the PCA Data: Similar to the method done above to cluster cryptos with Keans using original data, the same is done here using the PCA data. Here the K-means model is fitted with the PCA data, the clusters predicted and a column added for pca clusters. This was then viewed as a scatter plot:
 
## Visualise and compare the composite plots: Using the + operator, the hvplots and the scatter plots were respectively visualised side by side for the best value of k with the original data and the PCA data. Same was also done for the crypto clusters. My interpretation of the visual analysis is mentioned at the end of the assignment.
