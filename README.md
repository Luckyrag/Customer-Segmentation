# 🧠 Customer Segmentation using Clustering (K-Means & DBSCAN)

## 📌 Overview
This project focuses on performing customer segmentation based on **Annual Income** and **Spending Score** using unsupervised machine learning algorithms — **K-Means** and **DBSCAN**. The aim is to group similar customers together for targeted marketing strategies.

---

## 🗂️ Dataset
**Source**: Mall Customer Dataset

### Features:
- `CustomerID`: Unique identifier  
- `Gender`: Male/Female  
- `Age`: Age of the customer  
- `Annual Income (k$)`: Yearly income  
- `Spending Score (1-100)`: Based on customer behavior and shopping data  

---

## 🔍 Exploratory Data Analysis (EDA)
- `.head()`, `.info()`, `.describe()` for data overview  
- Categorical distribution (e.g., gender counts)  
- Pairplots & correlation heatmap  
- Spending behavior vs. income visualizations  

---

## 🤖 Clustering Models Used

### 1. K-Means Clustering
- Used **Elbow Method** to determine optimal clusters (`k = 5`)  
- Visualized results with cluster centers  
- Suitable for **spherical** & **compact** clusters  

### 2. DBSCAN Clustering
- Density-based algorithm  
- Does **not** require predefined number of clusters  
- Handles **noise** & **outliers** better  
- Visualized results using custom 2D plots  

---

## 📊 Visualization
- Scatter plots with cluster coloring  
- Cluster centers marked in red (for K-Means)  
- Comparison of K-Means vs DBSCAN clustering patterns  

---

## ⚖️ K-Means vs DBSCAN Comparison

| Metric           | K-Means             | DBSCAN                    |
|------------------|---------------------|----------------------------|
| Shape Handling   | Spherical only      | Arbitrary shapes          |
| Outlier Detection| ❌                  | ✅                         |
| Parameters       | `n_clusters (k)`    | `eps`, `min_samples`      |
| Speed            | Fast                | Slower (on large datasets)|
| Cluster Count    | Must define `k`     | Found automatically       |

---

## 📁 Project Structure
```text
customer-segmentation/
├── data/
│   └── customer_data.csv                 # Dataset file
├── visuals/
│   ├── kmeans_clusters.png              # Visualization from K-Means
│   └── dbscan_clusters.png              # Visualization from DBSCAN
├── customer_segmentation.ipynb          # Main Jupyter notebook
├── README.md                             # Project README (detailed doc)
├── requirements.txt                      # List of required packages
├── LICENSE                               # MIT License file
└── .gitignore                            # Files to ignore by Git
```

## ✅ Requirements

Install all dependencies using pip:

```bash
pip install pandas matplotlib seaborn scikit-learn dtale
```
## 🚀 How to Run
Clone the repo

Run the notebook: customer_segmentation.ipynb

Experiment with K-Means and DBSCAN on other features too

## 📈 Future Enhancements
Try Agglomerative or Gaussian Mixture Clustering

Use PCA for dimensionality reduction

Build a Flask dashboard for business use

## 📬 Contact
Name: Lokesh Raghuwanshi

Email: luckyraghuwanshi74@gmail.com

LinkedIn: www.linkedin.com/in/lokeshraghuwanshi74

GitHub: https://github.com/Luckyrag
