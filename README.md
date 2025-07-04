# **Task-8: Clustering with K-Means**

### **Dataset**

* **File:** `Mall_Customers.csv`
* **Location:** Local upload
* **Target Variable:** Unsupervised task (no target variable)

### **Tools & Libraries**

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

### **Steps Performed**

1. **Loaded the dataset**
   * Removed unnecessary columns (`CustomerID`).
   * Used `head()` and `info()` to inspect the data.
2. **Preprocessed the data**
   * Encoded `Gender` using Label Encoding.
   * Applied StandardScaler to normalize all features.
3. **Applied the Elbow Method**
   * Calculated WCSS for K values from 1 to 10.
   * Plotted Elbow Curve to determine optimal number of clusters (K).
4. **Trained K-Means Clustering Model**
   * Chose optimal `K=5` based on elbow plot.
   * Used `KMeans` from Scikit-learn to assign cluster labels.
5. **Evaluated Clustering Quality**
   * Calculated **Silhouette Score** to evaluate how well the clusters are separated.
6. **Visualized Clusters using PCA**
   * Applied **PCA** to reduce dimensions to 2D for visualization.
   * Plotted scatter plot with clusters color-coded.

### **Output**

* **Elbow Plot:**
  * Helped choose the optimal number of clusters.
* **Cluster Labels:**
  * Assigned to each customer for segmentation.
* **Silhouette Score:**
  * Quantified how well the clustering grouped similar customers.
* **Cluster Visualization:**
  * Displayed customer groups in 2D PCA space.
* **Conclusion:**
  * K-Means successfully grouped customers into distinct clusters.
  * Useful for customer segmentation based on behavior and spending patterns.
