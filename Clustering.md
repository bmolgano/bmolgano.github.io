Clustering Analysis
(a) Overview
Clustering is an unsupervised machine learning technique that groups similar data points together based on their features. Unlike supervised methods, clustering does not require labeled outcomes. There are two primary types of clustering, 
partitional clustering which divides data into k non-overlapping clusters based on a defined distance metric, and hierarchical Clustering which builds a tree by successively merging or splitting clusters. For this analysis, the euclidean 
distance for k-means and cosine similarity for hierarchical clustering were utilized. Clustering helps uncover natural groupings within Colorado population projections and demographics, allowing for deeper 
insight into regional service needs for behavioral health.

(b) Data Preparation
Clustering requires unlabeled, numeric input data. I extracted a subset of demographic and population projection features from my cleaned dataset and scaled it using StandardScaler to ensure uniform contribution across variables.
Below is a sample of the data used:
*** Add Dataset

(c) Clustering Code
I used Python (Google Colab) to implement both k-means and hierarchical clustering.

(d) Results
Silhouette Analysis:
Based on silhouette scores, the optimal number of clusters was k = 3.

K-Means Clustering Output:
The 2D PCA projection of clusters reveals distinct groupings:

Hierarchical Clustering:
The dendrogram indicates that the data can naturally be grouped into 3 clusters as well, supporting the k-means result.

(e) Conclusions
This clustering analysis revealed three distinct groups within the Colorado population projection dataset. These clusters may represent counties or regions with similar demographic growth patterns or health service demand. 
Understanding these groupings can inform how resources are allocated or how mental health services are targeted based on region-specific needs.

