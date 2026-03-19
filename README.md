# ACSWILDA26_01B_T5
This Repository contains the project related to ACS WIL Program Data Analysis Track

# 📊 Customer Clustering Analysis (K-Means)

This project focuses on applying data preprocessing and K-Means clustering to segment customers into meaningful groups based on their demographic and service usage characteristics.

---

## 📌 Project Overview

The goal of this project is to:

- Prepare and clean a real-world customer dataset
- Apply preprocessing techniques such as encoding and scaling
- Use K-Means clustering to identify customer segments
- Visualise and interpret the resulting clusters

This analysis helps uncover patterns in customer behaviour that can support business decision-making, such as targeted marketing and customer retention strategies.

---

## 🗂️ Project Structure

```text
Data_Preparation/
├── Datasets/
├── Code/
└── Documentation/

Clustering_Analysis/
├── Datasets/
├── Code/
├── Model/
├── Visualisations/
└── Documentation/

```
---

## ⚙️ Technologies Used

- Python 🐍
- Pandas & NumPy
- Scikit-learn
- Matplotlib & Seaborn
- Jupyter Notebook

---

## 🧹 Data Preparation

The dataset was preprocessed using a structured pipeline:

- Removed duplicate records
- Checked and handled missing values
- Encoded categorical variables using **One-Hot Encoding**
- Scaled numerical features using **StandardScaler**
- Split dataset into training (80%) and testing (20%)

### 📁 Output Files:
- `train_preprocessed.csv`
- `test_preprocessed.csv`
- `full_preprocessed_dataset.csv`

---

## 🤖 Clustering Analysis

### 🔹 Optimal Number of Clusters

The **Elbow Method** was used to determine the optimal number of clusters.

- Inertia values were calculated for k = 1 to 10
- The curve showed a clear bend at **k = 3**
- Therefore, **3 clusters** were selected

---

### 🔹 K-Means Model

A K-Means model was trained using:

```python
KMeans(n_clusters=3, random_state=42, n_init=10)
