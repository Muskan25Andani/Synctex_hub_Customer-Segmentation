# 📊 Synctex_Hub_Customer Segmentation Using K-Means Clustering

## 📌 Project Overview

This project implements **customer segmentation** using **unsupervised machine learning (K-Means clustering)**. The goal is to divide customers into distinct groups based on their **Age, Annual Income, and Spending Score**, enabling businesses to target marketing strategies more effectively.

---

## 📂 Dataset

* **Source:** Mall Customers Dataset (commonly available on Kaggle)
* **Features Used:**

  * `Age` – Customer age
  * `Genre` – Gender (Male/Female)
  * `Annual Income (k$)` – Annual income in thousands
  * `Spending Score (1-100)` – Customer spending behavior

---

## 🎯 Project Objectives

1. Load and explore the customer dataset.
2. Encode categorical data (Gender column).
3. Scale numerical features for clustering.
4. Determine the optimal number of clusters using the **Elbow Method**.
5. Apply **K-Means clustering** to segment customers.
6. Analyze and profile each cluster.
7. Save the segmented dataset for future analysis.

---

## ⚙️ Project Workflow

### 1️⃣ Data Loading

* Load the dataset from a CSV or ZIP file using `pandas`.

### 2️⃣ Data Preprocessing

* Handle missing values.
* Encode `Genre` column: Male → 0, Female → 1.
* Select features: `Age`, `Annual Income`, `Spending Score`.
* Standardize features using `StandardScaler`.

### 3️⃣ Determine Optimal Clusters

* Use the **Elbow Method** by plotting WCSS (Within-Cluster Sum of Squares) for k=1 to 10.

### 4️⃣ K-Means Clustering

* Apply K-Means with the optimal number of clusters (e.g., 5).
* Assign cluster labels to the dataset.

### 5️⃣ Cluster Analysis

* Group customers by clusters and calculate mean values of features.
* Understand the characteristics of each cluster (age, income, spending behavior).

### 6️⃣ Save Results

* Export the segmented dataset to `customer_segments.csv` for future use.

---

## 📊 Libraries Used

* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn

---

## 📁 Project Structure

```
CustomerSegmentation/
│── archive.zip (dataset)
│── customer_segmentation.py (main code)
│── customer_segments.csv (segmented output)
│── README.md
```

---

## 💡 Outcomes

* Customers are segmented into distinct clusters.
* Each cluster represents a group of customers with similar **age, income, and spending behavior**.
* Provides actionable insights for **marketing strategies** and **customer targeting**.

---

## 🚀 Future Enhancements

* Visualize clusters in 2D/3D plots.
* Apply other clustering techniques like **DBSCAN** or **Hierarchical Clustering**.
* Integrate demographic or purchase history for richer segmentation.

---
