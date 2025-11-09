## Mall Customers Clustering

This repository contains a clustering analysis of mall customer data to identify distinct customer segments. The goal is to help a mall understand its customers better and tailor marketing strategies to different groups.

### Project Structure

*   `Mall_Customers_Clustering.ipynb`: This Jupyter Notebook contains the complete Python code for data loading, preprocessing, exploratory data analysis (EDA), clustering (using K-Means), and visualization of the results.
*   `Mall_Customers.csv`: The dataset used for this analysis. It contains information about mall customers, including age, gender, annual income, and spending score.

### Analysis Steps

The analysis performed in the notebook includes:

1.  **Data Loading and Initial Inspection**: Loading the `Mall_Customers.csv` dataset and performing initial checks like viewing the first few rows, checking data types, and looking for missing values.
2.  **Exploratory Data Analysis (EDA)**:
    *   Univariate analysis of features like Age, Annual Income, and Spending Score using histograms and box plots.
    *   Bivariate analysis to understand relationships between features, for example, scatter plots of Annual Income vs. Spending Score.
    *   Analysis of customer distribution by Gender.
3.  **Feature Scaling**: Scaling numerical features to ensure that all features contribute equally to the clustering process.
4.  **Optimal Number of Clusters (K-Means)**: Using the Elbow Method to determine the optimal number of clusters for the K-Means algorithm.
5.  **K-Means Clustering**: Applying the K-Means algorithm with the chosen number of clusters to segment the customers.
6.  **Visualization of Clusters**: Visualizing the identified clusters, typically in a 2D scatter plot (e.g., Annual Income vs. Spending Score), with different colors representing different clusters.
7.  **Cluster Profiling**: Analyzing the characteristics of each cluster to understand the typical customer profile within each segment.

### How to Run the Notebook

To run the analysis yourself, follow these steps:

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/Abdelrahman-Shamikh/mall-customers-clustering.git
    ```
2.  **Navigate to the project directory**:
    ```bash
    cd mall-customers-clustering
    ```
3.  **Install the required libraries**:
    You can install them using pip:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
4.  **Open the Jupyter Notebook**:
    ```bash
    jupyter notebook Mall_Customers_Clustering.ipynb
    ```
    This will open the notebook in your web browser, and you can run the cells sequentially to reproduce the analysis.

### Results and Insights

The clustering analysis aims to reveal distinct groups of customers based on their spending habits and income. For example, some common segments found might include:

*   **Low Income, Low Spending**: Frugal customers.
*   **High Income, High Spending**: Target customers for luxury items.
*   **Medium Income, Medium Spending**: Average customers.
*   **High Income, Low Spending**: Potential for targeted promotions to encourage spending.
*   **Low Income, High Spending**: Careful analysis needed, perhaps impulse buyers or those spending beyond their means.

By understanding these segments, the mall can:

*   Develop **targeted marketing campaigns** for each group.
*   Optimize **store layouts and product placements**.
*   Improve **customer service strategies**.
*   Identify **opportunities for new promotions or loyalty programs**.

### Example Visualization of Clusters

Here's an example of what a visualization of the clusters might look like:

