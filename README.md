# 👥 Customer Segmentation using KMeans + Power BI Dashboard 📊

This project focuses on segmenting customers into distinct groups using **KMeans clustering** based on their attributes and behaviors. The goal is to help businesses understand their customer base better and provide **tailored strategies** and **recommendations** for each segment.

Additionally, a **Power BI dashboard** was created to visualize key insights, trends, and segment profiles for improved business decision-making.

---

## 📌 Features
  
- 📊 Customer segmentation using **KMeans clustering**  
- 🧩 Detailed cluster profiling and interpretation  
- 💡 Tailored business suggestions for each customer segment  
- 🧠 Interactive **Power BI dashboard** 

---

## 🧠 ML Workflow

### 1. 🗃️ Data Collection
- Dataset downloaded from Kaggle: **Customer Personality Analysis**
- Format: `.csv` file extracted from ZIP

### 2. 🧹 Data Preprocessing
- Removed unnecessary columns (`ID`, `Z_CostContact`, `Z_Revenue`, etc.)
- Converted `Dt_Customer` to datetime format
- Dropped rows with missing values
- Filtered out outlier ages (`Age > 90`)

### 3. 🛠️ Feature Engineering
- Derived `Age` from `Year_Birth`
- Calculated `Years_Shopping` from `Dt_Customer`
- Combined product spendings into a `Spent` feature
- Calculated `Children` by summing `Kidhome` and `Teenhome`
- Simplified and encoded categorical features like `Marital_Status` and `Education`

### 4. ⚖️ Data Scaling
- Dropped marketing response-related columns not needed for clustering
- Applied `StandardScaler` to normalize numeric features

### 5. 📉 Dimensionality Reduction
- Used **PCA** (Principal Component Analysis) to reduce features to 2D for visualization

### 6. 📊 Clustering
- Implemented **KMeans Clustering** on the scaled data
- Determined optimal number of clusters using the **Elbow Method**
- Assigned cluster labels to each customer

### 7. 🔍 Cluster Analysis & Interpretation
- Analyzed key statistics per cluster to derive customer personas
- Generated segment-specific business recommendations

### 8. 📈 Visualization
- Created an interactive **Power BI Dashboard** to:
  - Visualize customer segments
  - Compare features across clusters
  - Display actionable insights for business stakeholders

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
