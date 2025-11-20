# PRODIGY_ML_02 — Customer Segmentation using K-Means Clustering
---

This repository contains **Task-02 of my Machine Learning Internship at Prodigy InfoTech**.  
The project focuses on using the **K-Means Clustering algorithm** to segment mall customers based on their shopping behavior and spending habits.

Customer segmentation helps businesses categorize customers into meaningful groups and design better marketing strategies, personalized offers, and product recommendations.

---

## 📌 Project Summary
Customer segmentation is an important unsupervised learning technique.  
In this project, I worked with the popular **Mall Customers Dataset** to identify natural customer groups based on:

- Annual Income (k$)  
- Spending Score (1–100)  
- Age & Gender (for EDA)

This segmentation answers questions like:
- Who are the high-value customers?  
- Who spends less?  
- Which customers should be targeted?  

---

## 📂 Dataset Information

The dataset includes the following features:

| Feature | Description |
|--------|-------------|
| CustomerID | Unique customer identifier |
| Gender | Male / Female |
| Age | Customer age |
| Annual Income (k$) | Yearly income |
| Spending Score | Behavior-based spending score |

📌 The dataset is included inside the repository under the `dataset/` folder.

---

## 🧰 Technologies Used

- Python  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  
- Scikit-Learn  

---

## 🚀 How to Run

### **1️⃣ Clone the repository**
```bash
git clone https://github.com/your-username/PRODIGY_ML_02.git
```

### **2️⃣ Navigate to the project directory**
```bash
cd PRODIGY_ML_02
```

### **3️⃣ Install the required dependencies**
```bash
pip install -r requirements.txt
```

### **4️⃣ Launch the Jupyter Notebook**
```bash
jupyter notebook Task2_ML.ipynb
```

---

## 📊 Methodology

### ✔️ 1. Data Preprocessing
- Loaded dataset using Pandas  
- Checked missing values  
- Visualized basic distributions  
- Selected relevant features for clustering  

### ✔️ 2. Feature Selection
Used:  
- Annual Income  
- Spending Score  

These two show the clearest separation for clusters.

### ✔️ 3. Finding Optimal Clusters (Elbow Method)
- Calculated WCSS for k = 1 to 10  
- Identified the elbow at **k = 5**  

### ✔️ 4. Applying K-Means
- Initialized K-Means with 5 clusters  
- Predicted cluster labels  
- Extracted cluster centroids  

### ✔️ 5. Visualization
- Scatter plot of all clusters  
- Highlighted centroids  
- Color-coded segmentation  

---

## 📈 Results & Interpretation

The algorithm identified **5 distinct customer segments**:

1️⃣ Cluster 1 — Low Income, Low Spending  
2️⃣ Cluster 2 — Average Income, Average Spending  
3️⃣ Cluster 3 — High Income, Low Spending  
4️⃣ Cluster 4 — High Income, High Spending *(premium customers)*  
5️⃣ Cluster 5 — Low Income, High Spending  

These clusters help businesses identify:
- Target customers  
- Offer-sensitive groups  
- Loyal/premium buyers  
- Budget-conscious customers  

---

## 🗂️ Repository Structure

```
PRODIGY_ML_02/
│
├── Task2_ML.ipynb
├── README.md
├── requirements.txt
│
├── dataset/
│   └── Mall_Customers.csv
│
├── models/
│   └── kmeans_model_task2.joblib
│
└── screenshots/
    ├── elbow_method.png
    └── clusters.png
```

---

## 📜 License
This project is open-source and available for educational use.

