# Iris Flower Clustering Using K-Means  

## Overview  
This project applies **Unsupervised Learning** techniques, specifically **K-Means Clustering**, to group the **Iris dataset** into distinct clusters. The **Elbow Method** is used to determine the optimal number of clusters, and the results are visualized for better interpretation.  

## Machine Learning Approach  
- **Unsupervised Learning**: No labeled target variable; the model finds patterns and groups data points based on similarity.  
- **K-Means Clustering**: A clustering algorithm that assigns data points into `k` groups based on feature similarities.  

## Steps in the Code  

### 1. Load the Iris Dataset  
- Uses **Scikit-learn's `datasets` module** to load the **Iris dataset**.  
- Converts it into a **pandas DataFrame**.  

### 2. Determine the Optimal Number of Clusters (Elbow Method)  
- Computes **Within-Cluster Sum of Squares (WCSS)** for different `k` values.  
- Uses **Elbow Method** to find the best `k`.  

### 3. Apply K-Means Clustering  
- Trains a **K-Means** model using `k=3` (as determined by the Elbow Method).  
- Predicts cluster labels for each data point.  

### 4. Visualizing the Clusters  
- Uses **Matplotlib** to plot clusters and their **centroids**.  
- Different colors represent the three **Iris species**:  
  - **Iris-setosa** (black)  
  - **Iris-versicolor** (blue)  
  - **Iris-virginica** (pink)  
- Cluster **centroids** are marked in **green**.  

## Technologies Used  
- Python  
- Pandas (Data Handling)  
- NumPy  
- Scikit-Learn (Machine Learning)  
- Matplotlib (Data Visualization)  

## How to Run  
1. Install dependencies:  
   ```bash
   pip install pandas numpy scikit-learn matplotlib
