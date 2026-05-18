# Requirement
The data set refers to clients of a wholesale distributor. It includes the annual spending in monetary units (m.u.) on diverse product categories. Perform customer segmentation using clustering techniques on wholesale spending data.

# EDA:
There are 8 features, out of which 6 are numerical and 2 are Categorical. 

Numerical Features:'Fresh', 'Milk', 'Grocery', 'Frozen', 'Detergents_Paper', 'Delicassen'
Categorical Features: 'Channel', 'Region'


# Following clustering techniques are used:
KMeans
DBScan
Agglomerative
Execution:
Used elbow method to find the number of clusters:



# Modeled the data with KMeans/ DbScan/ Agglomerative clustering techniques and here are the summary of the results:


1. Got Best Silhouette Score when the data is transformed with StandardScalar and modeled with Kmeans - 0.3325
2. This wholesale dataset is highly overlapping, so DBScan is not performing well with this dataset.
3. Clusters generated from each model are visualized with PCA with 2 components. Though the Silhouette score of the model is low after removing outliers, it is observed from the PCA scatterplot that the clusters are better separated.
4. After careful consideration, it is decided to use the KMeans model created with data after outlier removal for final clustering


# Data visualisation with PCA:



# Result:
Average Spending by Clusters:







Cluster 0: Most spendings are in Grocery, followed by Fresh, Milk, Detergents_Paper and  Delicatessen, Lowest spending in Frozen.
Cluster 1: Most spendings are in Fresh, followed by Grocery, Milk, Frozen and Delicatessen, Lowest spending in Detergents_Paper.
Cluster 2: Most spendings are in Grocery, followed by Fresh and Milk, Detergents_Paper and Frozen  Lowest spending in Delicatessen.
Cluster 3: Most spendings are in Fresh, followed by Frozen, Grocery, Milk and Delicatessen, Lowest spending in Detergents_Paper.












# Conclusion:
Cluster Distribution by Channel:







Horeca Spendings are mostly in cluster 1 and 3, which means most spendings are in Fresh. Lowest in Detergents_Paper.
Retail Spendings are mostly in cluster 0 and 2, which means most spending are in Grocery, lowest in Frozen and Delicatessen.


# Future Action:
Business can promote more Fresh products for HoReCA customers, probably add more discounts and promotions. Retail customers spend more on Grocery, so business should promote more on Grocery products for Retail customers.
