# 👥 Customer Segmentation using KMeans + Power BI Dashboard 📊

This project focuses on segmenting customers into distinct groups using **KMeans clustering** based on their attributes and behaviors. The goal is to help businesses understand their customer base better and provide **tailored strategies** and **recommendations** for each segment.

Additionally, a **Power BI dashboard** was created to visualize key insights, trends, and segment profiles for improved business decision-making.

---

## 📌 Features
  
-  Customer segmentation using **KMeans clustering**  
-  Detailed cluster profiling and interpretation  
-  Tailored business suggestions for each customer segment  
-  Interactive **Power BI dashboard** 

---

## 🧠 ML Workflow

### 1. Data Collection
- Dataset downloaded from Kaggle: **Customer Personality Analysis**
- Format: `.csv` file extracted from ZIP

### 2. Data Preprocessing
- Removed unnecessary columns (`ID`, `Z_CostContact`, `Z_Revenue`, etc.)
- Dropped rows with missing values
- Filtered out outlier ages (`Age > 90`)

### 3. Feature Engineering
- Derived `Age` from `Year_Birth`
- Calculated `Years_Shopping` from `Dt_Customer`
- Combined product spendings into a `Spent` feature
- Calculated `Children` by summing `Kidhome` and `Teenhome`
- Simplified and encoded categorical features like `Marital_Status` and `Education`

### 4. Data Scaling
- Dropped marketing response-related columns not needed for clustering
- Applied `StandardScaler` to normalize numeric features

### 5. Dimensionality Reduction
- Used **PCA** (Principal Component Analysis) to reduce features to 2D for visualization

### 6. Clustering
- Implemented **KMeans Clustering** on the scaled data
- Determined optimal number of clusters using the **Elbow Method**
- Assigned cluster labels to each customer

---

## 📊 Dashboard Preview
[Dashboard Preview](https://github.com/Shreiya-Muthuvelan/Customer-Segmentation/blob/main/Purchase%20Insights%20Dashboard.pdf)

[Download the interactive .pbix file](https://github.com/Shreiya-Muthuvelan/Customer-Segmentation/blob/main/Purchase%20Insights%20Dashboard.pbix)

---

## 📄 Cluster Insights & Strategy Report
[View PDF Report](https://github.com/Shreiya-Muthuvelan/Customer-Segmentation/blob/main/Customer_Segmentation_Report.pdf)

---

## 🗂️ Technologies Used
- Python
- Scikit-Learn
- Pandas
- Numpy
- Matplotlib
- Seaborn
- KMeans
- PCA
- Power BI

---
## 🪪 License
MIT License © Shreiya Muthuvelan See [LICENSE](LICENSE) for more details.
