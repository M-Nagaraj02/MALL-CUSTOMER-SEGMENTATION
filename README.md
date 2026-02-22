# 🛍️ Mall Customer Segmentation Using K-Means Clustering
---
# Overview

This project performs Customer Segmentation using the K-Means Clustering Algorithm, an unsupervised machine learning technique.
It groups mall customers into different clusters based on their Annual Income and Spending Score, helping businesses understand customer behavior and improve marketing strategies.

---
# Dataset

Mall Customers Dataset ```python (Mall_Customers.csv)```
 * Total Records: 200
 * Total Features: 5
Features used for clustering:
 * Annual Income (k$)
 * Spending Score (1–100)
```python
import pandas as pd
df = pd.read_csv("Mall_Customers.csv")
```
---
# Methodology

* Selected important features:
     * Annual Income
     * Spending Score
* Applied StandardScaler for feature scaling
* Used Elbow Method to determine optimal number of clusters
* Applied K-Means Algorithm
* Added predicted cluster labels to dataset
* Visualized clusters using scatter plot
---
# Algorithm Used

* K-Means Clustering
   * Random centroid initialization
   * Iterative optimization
   * Minimizes Within-Cluster Sum of Squares (WCSS)
```python
from sklearn.cluster import KMeans
kmeans = KMeans(n_clusters=7, random_state=42)
```
---
# Results

* Used Elbow Method to find optimal K value
* Selected 7 clusters
* Customers successfully grouped into meaningful segments
* Clear visualization using scatter plot

**Example segments:**

* High Income – High Spending
* High Income – Low Spending
* Low Income – High Spending
* Low Income – Low Spending

---
# Visualization

Elbow Method Graph – Used to determine optimal clusters
 <img width="571" height="455" alt="image" src="https://github.com/user-attachments/assets/fa4a2023-f87f-4e3c-9caf-d808b089916e" />
 
Customer Cluster Scatter Plot – Visual representation of segmented customers
<img width="578" height="455" alt="image" src="https://github.com/user-attachments/assets/b4bc6f55-ff06-4fd9-8264-84883cd3038c" />

---
# Project Structure

MALL-CUSTOMER-SEGMENTATION/
 * │── Mall_Customers.csv
 * │── Mall_Customer_Segmentation.ipynb
 * │── README.md
---
#Author

**Nagaraj M**

GitHub: https://github.com/M-Nagaraj02
