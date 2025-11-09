# mall-customers-clustering

---

# Customer Segmentation Clustering Analysis

**Acknowledgements:** 
Eng. Baraa Abu Sallout – for guidance and support;
Robert Kwiatkowski – original author of the Kaggle notebook that inspired and was edited for this project.

---

## Overview

This repository contains a clustering analysis of customer data (Mall Customers), aimed at segmenting customers based on demographic and behavioral features, such as **Gender**, **Age**, **Annual Income (k$)**, and **Spending Score (1–100)**. The objective is to identify distinct customer groups for better marketing and business strategy insights.

Three clustering algorithms were applied and compared:

* **K-Means Clustering**
* **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**
* **Agglomerative Hierarchical Clustering (Ward’s Linkage Method)**

All features were standardized to ensure fair distance-based clustering.

---

## Key Visualizations

1. **Elbow Method Plot**
   Determines the optimal number of clusters for K-Means. The "elbow" was observed around **k = 5**, indicating 5 natural customer segments.

2. **K-Means Cluster Visualization**
   Scatter plot of Annual Income vs Spending Score. Clusters are well-separated and circular.

3. **DBSCAN Visualization**
   Scatter plot showing core samples and noise points. Dense customer groups were identified, while low-density customers were marked as outliers.

4. **Hierarchical Clustering Dendrogram**
   Shows hierarchical cluster structure. Clear separation suggests **3 major clusters**.

5. **3D Scatter Plot**
   Visualizes clusters across Age, Annual Income, and Spending Score for a holistic view.

---

## Insights

* **K-Means Clustering (k=5)** identified five distinct customer segments:

  1. High-income, high-spending customers (premium group)
  2. Low-income, high-spending customers (impulsive buyers)
  3. High-income, low-spending customers (conservative spenders)
  4. Average-income, moderate-spending customers
  5. Low-income, low-spending customers

* **DBSCAN** highlighted dense clusters and outliers. Sensitive to parameter tuning (`eps` and `min_samples`), it effectively detected noise but was less consistent for evenly distributed data.

* **Agglomerative Hierarchical Clustering** grouped customers into **3–4 broader segments**, capturing larger behavioral categories.

* **Key features influencing clusters**: Spending Score and Annual Income.

---

## Reflection

* **K-Means**: Most interpretable, well-defined clusters, but assumes spherical shapes.
* **DBSCAN**: Effective for irregular clusters and outlier detection, but requires careful parameter tuning.
* **Agglomerative Clustering**: Provides hierarchical insight and clear dendrograms; computationally heavier on large datasets.

**Challenges:**

* Selecting the optimal number of clusters.
* Properly scaling features to ensure equal contribution.
* Visualizing high-dimensional data in 2D/3D.

**Conclusion:**
Combining multiple clustering methods provides a comprehensive understanding of customer segmentation. K-Means offers actionable segments, hierarchical clustering validates results, and DBSCAN identifies outliers and irregular patterns.

---

## How to Run

1. Install required packages:

   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn
   ```
2. Load the dataset: `Mall_Customers.csv`
3. Run the notebook `customers-clustering-k-means-dbscan-and-ap.ipynb` to reproduce the analysis and visualizations.

---

## License

This project is open-source for educational and analytical purposes.

