# LAB-Unsupervised-Learning-Clustering

![Image](https://user-images.githubusercontent.com/970858/63474771-d6734700-c469-11e9-83bb-9429da563909.png)

# Mall Customers Dataset Clustering Analysis

## Introduction

In this project, we explore the strengths and limitations of two popular clustering algorithms: **K-Means** and **DBSCAN**. Using the **Mall Customers dataset**, which includes customer demographic and behavioral data, we will perform customer segmentation tasks. The goal is to understand how DBSCAN can overcome some limitations of traditional clustering methods like K-Means and to evaluate the performance of each algorithm using various clustering evaluation metrics.

## Setup Instructions

To run the notebook and reproduce the results, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/codeskills-ai/LAB-Unsupervised-Learning-Clustering.git
    cd LAB-Unsupervised-Learning-Clustering
    ```

2. **Create a virtual environment and install the required packages**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Start Jupyter Notebook**:
    ```bash
    jupyter notebook
    ```

## Steps in the Workflow

### Step 1: Data Load and Exploration

Load and explore the Mall Customers dataset to understand its structure and distribution. This step includes handling categorical variables and performing exploratory data analysis (EDA).

- **Load Dataset**: Import the necessary libraries and load the dataset.
- **EDA**: Perform descriptive statistics and visualize data distributions.
- **Handle Categorical Variables**: Convert the `Gender` column to numerical format using label encoding.

### Step 2: Feature Selection and Correlation Analysis

Prepare features for clustering by selecting relevant variables and analyzing their correlations.

- **Feature Selection**: Select `Age`, `Annual Income`, `Spending Score`, and the encoded `Gender` variable for clustering.
- **Correlation Analysis**: Compute and visualize the correlation matrix using a heatmap to understand feature relationships.

### Step 3: Data Visualization

Visualize the dataset in both 2D and 3D to understand the data distribution in multiple dimensions.

- **3D Scatter Plot**: Create an interactive 3D scatter plot to visualize the relationships between `Age`, `Annual Income`, and `Spending Score`.
- **2D Scatter Plot**: Create a 2D scatter plot to visualize the relationships between selected features.

### Step 4: K-Means Clustering

Apply K-Means clustering to the dataset and visualize the clustering results.

- **Apply K-Means**: Extract relevant features and apply K-Means clustering with 5 clusters.
- **Result Visualization**: Visualize the clustering results using 3D and 2D scatter plots.
- **Model Evaluation**: Evaluate the K-Means model using Silhouette Score and Davies-Bouldin Index.

### Step 5: DBSCAN Clustering

Apply DBSCAN clustering to the dataset and compare its results with those obtained from K-Means.

- **Apply DBSCAN**: Apply DBSCAN with initial `eps` and `min_samples` values.
- **Result Visualization**: Visualize the DBSCAN clustering results using 3D scatter plots.
- **Model Evaluation**: Evaluate the DBSCAN model using Silhouette Score and Davies-Bouldin Index.

### Step 6: Improving DBSCAN Results

Manually tune DBSCAN's `eps` and `min_samples` parameters to improve clustering performance.

- **Hyperparameter Tuning**: Perform a manual grid search to find the optimal `eps` and `min_samples`.
- **Evaluate Best Model**: Re-evaluate the model using the best parameters and visualize the results.

### Step 7: Comparison and Conclusion

Compare the performance of K-Means and DBSCAN using the best-tuned models and draw conclusions about their effectiveness for this dataset.

- **Model Comparison**: Compare the Silhouette Score and Davies-Bouldin Index of the final models.

### Additional Challenge (Optional)

For further exploration, try implementing hierarchical clustering and compare its results with K-Means and DBSCAN.