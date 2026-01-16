# Airbnb Clustering — Price‑Based Segmentation

This repository contains an **unsupervised learning project** on Airbnb listings data, focused on **price‑based clustering** of properties. The goal is to discover natural groupings of listings based on pricing and related features such as capacity, location, and quality indicators.

---

## 📁 Dataset

This project uses publicly available Airbnb listings data from **Inside Airbnb**.

🔗 **Direct dataset download (London listings, 2025‑09‑14):**  
https://data.insideairbnb.com/united-kingdom/england/london/2025-09-14/data/listings.csv.gz

> The dataset includes listing attributes such as price, room type, property type, availability, reviews, and location coordinates.

---

## 🎯 Objective

The goal of this project is to:

- Clean and preprocess the Airbnb listings dataset  
- Encode categorical features and scale numeric features  
- Apply PCA for visualization (and optionally for clustering stability)  
- Perform clustering (K‑Means) to segment listings into pricing tiers  
- Interpret clusters using summary statistics and visualizations  

This is a **purely unsupervised learning project** — there is no target variable and no train/test split.

---

## 🧾 Workflow Summary

1. **Load the dataset**
2. **Data cleaning**
   - Fix price formatting (remove currency symbols and commas)
   - Handle missing values (median imputation)
3. **Encoding**
   - One‑Hot Encoding for low‑cardinality categorical columns (e.g., `room_type`)
   - Frequency encoding for high‑cardinality columns (optional)
4. **Scaling**
   - StandardScaler for numeric features
5. **Dimensionality Reduction (Optional)**
   - PCA for 2D visualization
6. **Clustering**
   - Elbow method for selecting K
   - K‑Means clustering
7. **Cluster Interpretation**
   - Cluster profiling (mean/median price and other key features)
   - Visualizations (PCA scatter plots, boxplots)

---

## 🚀 How to Run

### 1) Clone the repository
```bash
git clone https://github.com/Naman0911/AirBnb-Clustering.git
cd AirBnb-Clustering
```

### 2) Download dataset
Download from:
```text
https://data.insideairbnb.com/united-kingdom/england/london/2025-09-14/data/listings.csv.gz
```

Place it in a folder such as:
```text
data/listings.csv.gz
```

### 3) Install dependencies
```bash
pip install -r requirements.txt
```

### 4) Run notebook / script
Open Jupyter Notebook:
```bash
jupyter notebook
```

Run your clustering notebook/script and generate results.

---

## 📊 Results You Can Generate

- Elbow curve (Inertia vs K)
- PCA 2D plot colored by cluster
- Cluster-wise mean/median price comparison
- Cluster profiling table

---

## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Scikit‑learn
- Matplotlib, Seaborn

---

## 🙌 Acknowledgements

- Dataset: **Inside Airbnb** (http://insideairbnb.com)

---

## 📄 License

This project is for educational purposes.
