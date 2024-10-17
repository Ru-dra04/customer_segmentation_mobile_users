# Customer Segmentation of Mobile Users – Data Science Project
This project aims to segment mobile users based on their usage patterns, device characteristics, and demographic information using KMeans clustering. The project covers data preprocessing, feature engineering, clustering, and several ad-hoc analyses, including Principal Component Analysis (PCA) for visualization and cluster centroid analysis. The insights derived from this project can help businesses make data-driven decisions for personalized services, product development, or targeted marketing strategies.

# Project Overview
##### -> Goal: Segment mobile users into distinct groups (clusters) based on their behavior and characteristics.
##### -> Methodology: Data preprocessing and feature scaling.
##### -> Applying KMeans clustering to create segments.
##### -> Visualizing clusters using PCA and analyzing key patterns in the data.
##### ->  Performing ad-hoc analyses such as summary statistics, boxplots, correlation analysis, and optimal cluster determination using the elbow method.


# Dataset
The dataset contains various attributes of mobile users:

![image](https://github.com/user-attachments/assets/66a500dd-4c14-4ebf-aa56-016323cd3928)


# Project Structure
## 1. Data Preprocessing
To ensure the dataset is ready for clustering, categorical variables such as Operating System and Gender are converted into numerical values.

Operating System: Android = 0, iOS = 1
Gender: Male = 0, Female = 1
This step also involves scaling the features using StandardScaler to normalize them, which is important for distance-based clustering algorithms like KMeans.

![image](https://github.com/user-attachments/assets/53a5f096-efe6-4d24-bbf7-46561b20f149)

## 2. Clustering with KMeans
The KMeans algorithm is used to group users into clusters based on their app usage patterns, battery consumption, and demographic factors. In this example, the data is clustered into 3 groups, but the number of clusters can be fine-tuned using the Elbow Method.

![image](https://github.com/user-attachments/assets/6bbccd75-1451-4e25-85e2-5c2a0eedb4da)

## 3. Principal Component Analysis (PCA)
PCA is applied to reduce the dimensionality of the dataset, making it easier to visualize the clusters in 2D. This technique is useful for understanding how distinct the clusters are in terms of key features.

![image](https://github.com/user-attachments/assets/75209403-594c-4d5a-b80a-b2faf432d69d)

![image](https://github.com/user-attachments/assets/67174605-6ff2-472b-b883-10d02e78219c)

## 4. Ad-hoc Analysis
Various ad-hoc analyses are performed to gain deeper insights into each cluster, including:

#### Summary Statistics: Understanding the average feature values per cluster.
#### Boxplots: Visualizing the spread of key features like App Usage Time and Battery Drain across clusters.
#### Correlation Analysis: Exploring relationships between different features.
#### Cluster Centroid Analysis: Identifying the key characteristics of users within each cluster by analyzing the cluster centroids.

![image](https://github.com/user-attachments/assets/035750b1-84f4-4a14-b4cd-ccdf30becfa4)

# Key Visualizations
#### PCA Visualization of Clusters: Displays how well the clusters are separated in a 2D space.
#### Cluster Centroid Bar Plot: Shows the average feature values per cluster, helping to distinguish the key characteristics of each segment.
#### Boxplots: Provide insight into the distribution of key features like App Usage Time and Battery Drain for each cluster.

# Elbow Method for Optimal Cluster Selection
The Elbow Method helps determine the optimal number of clusters by plotting the inertia (sum of squared distances) for different values of n_clusters. The "elbow" point in the plot indicates the ideal number of clusters.

![image](https://github.com/user-attachments/assets/b330d1d1-01a4-4f2a-83f8-1650045e8581)

![image](https://github.com/user-attachments/assets/25029e64-5368-4286-82cc-20f507010467)

# Conclusion
This project segments mobile users based on their usage patterns, providing insights into distinct customer groups. Businesses can leverage these insights to target specific customer segments more effectively and tailor their services/products to meet the needs of these groups.

# Installation and Usage Instructions

###  1. Clone the repository:
        git clone https://github.com/yourusername/customer-segmentation-mobile-users.git
###  2. Run the script:
        python customer_segmentation.py

# Dependencies
## Python 3.x
## pandas
## scikit-learn
## seaborn
## matplotlib

# Future Enhancements
### Implement additional clustering algorithms (e.g., Hierarchical Clustering, DBSCAN) to compare results.
### Fine-tune the number of clusters using advanced methods like Silhouette Score or Gap Statistics.
### Expand the dataset to include more detailed mobile usage behavior or demographic features.




