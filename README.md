#  Iris Flower Classification: Supervised vs Unsupervised Learning

This project presents a **comparative analysis** between **Logistic Regression** (supervised learning) and **K-Means Clustering** (unsupervised learning) on the **Iris flower dataset**. It explores model performance, decision boundaries, evaluation metrics, and application scenarios.

---

##  Abstract

The classification of Iris flowers is a foundational problem in machine learning. This study compares two contrasting approaches:
- **Logistic Regression**: Achieves ~97% accuracy using labeled data.
- **K-Means Clustering**: Achieves ~89% accuracy using unlabeled data after cluster-label mapping.

This highlights the trade-offs between label dependency and exploratory potential.

---

##  Objectives

1. Compare Logistic Regression and K-Means under identical preprocessing conditions.
2. Quantify post-cluster mapping accuracy for unsupervised learning.
3. Identify optimal use cases for each learning paradigm.

---

##  Dataset

- **Source**: `sklearn.datasets.load_iris()`
- **Classes**: Iris Setosa, Versicolor, Virginica
- **Features**:
  - Sepal length (cm)
  - Sepal width (cm)
  - Petal length (cm)
  - Petal width (cm)

---

##  Learning Models

###  Logistic Regression (Supervised)
- Multinomial (softmax) classifier
- Standardized features
- 70/30 train-test split
- Evaluated using: Accuracy, Confusion Matrix, Classification Report, Probabilities

###  K-Means Clustering (Unsupervised)
- k = 3 clusters
- Feature scaling
- Elbow method + silhouette analysis
- Post-hoc label mapping for accuracy
- Evaluated using: WCSS, Silhouette Score, Confusion Matrix

---

##  Results

| Metric                  | Logistic Regression | K-Means Clustering |
|-------------------------|---------------------|--------------------|
| Accuracy                | 97.3%               | 89.3%              |
| Data Requirement        | Labeled             | Unlabeled          |
| Use Case                | Predictive Modeling | Exploratory Analysis |
| Strengths               | High precision, confidence scores | No label dependency, intuitive grouping |
| Limitations             | Needs labels, linear assumptions | Sensitive to init, lower accuracy |

---

##  Visualizations

- 📌 Confusion Matrix (both models)
- 📌 Class Probabilities for LR
- 📌 Cluster plots with PCA
- 📌 Elbow curve (WCSS vs K)
- 📌 Silhouette analysis

---

##  Evaluation Metrics

- **Accuracy**
- **Confusion Matrix**
- **Silhouette Score (K-Means)**
- **Probability Distribution (Logistic Regression)**

---

##  Code Files

### `logistic_regression_iris.py`
Implements preprocessing, model training, accuracy evaluation, and visualization for Logistic Regression.

### `kmeans_iris.py`
Performs clustering, visualizations, elbow method, and evaluates clustering accuracy with mapped labels.

---

##  Conclusion

- **Logistic Regression** is highly effective with labeled data, ideal for production applications.
- **K-Means Clustering** is useful for exploratory analysis, especially when labels are unavailable.
- **Hybrid approaches** can combine the benefits of both for robust real-world implementations.

---

##  Future Work

- Introduce non-linear models (SVM, Random Forest, Neural Networks)
- Use real flower images with CNNs
- Explore semi-supervised learning
- Try alternative clustering methods (DBSCAN, Hierarchical)
- Feature engineering for class separation

---

Project developed as part of coursework on **Machine Learning / Pattern Recognition**.

---



---

> “Understanding when and how to use supervised or unsupervised methods is key to effective machine learning.”
