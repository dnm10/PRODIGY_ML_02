# PRODIGY_ML_02
# 🛃 Customer Segmentation with K-Means Clustering

This project performs unsupervised customer segmentation using the K-Means clustering algorithm on the [Kaggle Mall Customer Segmentation Data](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python).

---

## 🎯 Objective

To identify and group customers into distinct segments based on **spending behavior** and **annual income**, helping businesses tailor marketing strategies using **unsupervised machine learning**.

---

## 📁 Task Overview

- Perform K-Means clustering on customers based on:

    - **Annual Income (k$)**

    - **Spending Score (1-100)**

- Apply the **Elbow Method** to find the optimal number of clusters (k)

- Visualize the results using **Matplotlib and Seaborn**

- Handle known **MKL threading issue on Windows** with a proper workaround

---

## 🧠 Model Overview

- **Algorithm**: K-Means Clustering
- **Framework**: Scikit-learn
- **Evaluation Metric**: Within-Cluster Sum of Squares (WCSS / SSE), Elbow Method
- **Tools**: Python, Pandas, Matplotlib, Seaborn

---

## 🧯 Suppress OMP_NUM_THREADS Warning
A known issue occurs on Windows with MKL when using KMeans. Use the following methods to avoid repeated warnings:

**🔧 Temporary Fix**

Run this in Anaconda Prompt before launching the notebook:
```bash
  set OMP_NUM_THREADS=1
  jupyter notebook
```

**🛠 Permanent Fix**
Set a system environment variable:
    
  - **Variable name:** OMP_NUM_THREADS
  - **Value:** 1

Then **restart your system** to apply changes. 

---

## 📊 Results
The trained model segments customers into meaningful clusters. Outputs include:

- 📉 **Elbow Plot:** Helps identify the ideal number of clusters

- 🔵 **Cluster Scatter Plot:** Visualizes segmented customer groups

- 🎯 **Centroids:** Represents the center of each customer group

These insights can help businesses target specific customer segments more effectively.

---

## Author

- [@dnm10](https://github.com/dnm10)
