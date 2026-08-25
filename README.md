# AIML – Unsupervised Learning Models

## 📌 About the Project

This repository contains implementations of various **Unsupervised Machine Learning algorithms** using Python and popular machine learning libraries.

Unsupervised Learning is a type of Machine Learning where the model learns patterns and relationships from data without predefined target labels.

The following algorithms are implemented in this repository:

- Apriori
- DBSCAN Clustering
- ECLAT
- FP-Growth
- Hierarchical Clustering
- K-Means Clustering
- PCA (Principal Component Analysis)

---

## 📂 Project Structure

| No. | Algorithm | Type | Notebook |
|---|---|---|---|
| 1 | Apriori | Association Rule Mining | `Apriori.ipynb` |
| 2 | DBSCAN | Clustering | `DBSCAN_Clustering.ipynb` |
| 3 | ECLAT | Association Rule Mining | `ECLAT.ipynb` |
| 4 | FP-Growth | Association Rule Mining | `FP_Growth.ipynb` |
| 5 | Hierarchical Clustering | Clustering | `Hierarchical_Clustering.ipynb` |
| 6 | K-Means Clustering | Clustering | `K_Means_Clustering.ipynb` |
| 7 | PCA | Dimensionality Reduction | `PCA.ipynb` |

---

# 🧠 Algorithms Covered

## 1. Apriori

Apriori is an **association rule mining algorithm** used to discover frequently occurring itemsets and relationships between items.

### Applications
- Market Basket Analysis
- Product Recommendation
- Customer Purchase Analysis
- Cross-Selling

### Important Parameters

- **Support** – Frequency of an itemset in the dataset.
- **Confidence** – Probability that an item is purchased when another item is purchased.
- **Lift** – Measures the strength of an association between items.

### Notebook

`Apriori.ipynb`

---

## 2. DBSCAN Clustering

**DBSCAN (Density-Based Spatial Clustering of Applications with Noise)** is a clustering algorithm that groups points based on their density.

Unlike K-Means, DBSCAN does not require the number of clusters to be specified beforehand.

### Important Parameters

- `eps` – Maximum distance between two points to be considered neighbors.
- `min_samples` – Minimum number of points required to form a dense region.

### Advantages

- Detects clusters of arbitrary shape.
- Can identify noise and outliers.
- Does not require the number of clusters beforehand.

### Applications

- Geographic data analysis
- Anomaly detection
- Image processing
- Customer segmentation

### Notebook

`DBSCAN_Clustering.ipynb`

---

## 3. ECLAT

**ECLAT (Equivalence Class Transformation)** is an association rule mining algorithm.

It uses a **vertical data format**, where each item is associated with the transaction IDs in which it occurs.

### Advantages

- Efficient for frequent itemset mining.
- Uses transaction ID intersections.
- Can be faster than Apriori for certain datasets.

### Applications

- Market Basket Analysis
- Customer purchasing patterns
- Recommendation systems

### Notebook

`ECLAT.ipynb`

---

## 4. FP-Growth

**FP-Growth (Frequent Pattern Growth)** is an association rule mining algorithm that finds frequent itemsets without generating a large number of candidate itemsets.

It uses an **FP-Tree (Frequent Pattern Tree)** to represent transaction data.

### Advantages

- Faster than Apriori for many large datasets.
- Avoids candidate generation.
- Efficiently discovers frequent patterns.

### Applications

- Recommendation systems
- Market Basket Analysis
- Customer behavior analysis

### Notebook

`FP_Growth.ipynb`

---

## 5. Hierarchical Clustering

Hierarchical Clustering creates a hierarchy of clusters and is commonly visualized using a **dendrogram**.

There are two main approaches:

### Agglomerative Clustering

1. Initially, every data point is treated as an individual cluster.
2. The closest clusters are merged.
3. The process continues until the required hierarchy is formed.

### Applications

- Customer segmentation
- Biological data analysis
- Document clustering
- Image analysis

### Notebook

`Hierarchical_Clustering.ipynb`

---

## 6. K-Means Clustering

K-Means is one of the most widely used **clustering algorithms**.

It divides the dataset into `K` clusters based on the distance between data points and cluster centroids.

### Working Steps

1. Select the number of clusters `K`.
2. Initialize cluster centroids.
3. Assign each data point to the nearest centroid.
4. Calculate new centroids.
5. Repeat until the centroids converge.

### Evaluation

The **Silhouette Score** can be used to evaluate clustering quality.

A higher Silhouette Score generally indicates better-separated clusters.

### Applications

- Customer segmentation
- Image compression
- Pattern recognition
- Market analysis

### Notebook

`K_Means_Clustering.ipynb`

---

## 7. PCA

**PCA (Principal Component Analysis)** is a dimensionality reduction technique.

It transforms a dataset with many features into a smaller number of principal components while retaining as much important information as possible.

### Working Steps

1. Standardize the data.
2. Calculate the covariance structure.
3. Find principal components.
4. Sort components based on explained variance.
5. Transform the original dataset.

### Applications

- Dimensionality reduction
- Data visualization
- Feature extraction
- Noise reduction
- Machine Learning preprocessing

### Notebook

`PCA.ipynb`

---

# 🛠️ Technologies Used

- Python
- Jupyter Notebook
- Google Colab
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Mlxtend

---

# 📊 Model Evaluation

Since most algorithms in this repository are **unsupervised learning algorithms**, traditional classification accuracy is generally not appropriate.

Different evaluation techniques can be used depending on the algorithm.

| Algorithm | Evaluation Method |
|---|---|
| K-Means | Silhouette Score, Inertia |
| DBSCAN | Silhouette Score |
| Hierarchical Clustering | Silhouette Score, Dendrogram |
| PCA | Explained Variance Ratio |
| Apriori | Support, Confidence, Lift |
| ECLAT | Support, Confidence, Lift |
| FP-Growth | Support, Confidence, Lift |

> **Note:** Accuracy is normally used for supervised classification problems where true labels are available. For clustering, metrics such as Silhouette Score are more appropriate.

---

# 📈 Expected Outputs

The notebooks demonstrate results using tables and visualizations such as:

- Cluster plots
- Dendrograms
- Elbow Method graphs
- Silhouette analysis
- PCA visualization
- Frequent itemsets
- Association rules
- Support, Confidence and Lift values

---

# 🚀 How to Run

## Option 1 – Google Colab

1. Open the required `.ipynb` notebook.
2. Upload the required dataset.
3. Open the notebook using Google Colab.
4. Run the cells sequentially.

## Option 2 – Jupyter Notebook

Install the required libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn mlxtend openpyxl
