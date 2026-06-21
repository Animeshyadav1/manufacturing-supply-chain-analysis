# 🏭 End-to-End Manufacturing Supply Chain Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0-green)
![Scikit--Learn](https://img.shields.io/badge/Scikit--Learn-1.3-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

A complete end-to-end **Supply Chain Analysis** project using Python — covering Exploratory Data Analysis, Feature Engineering, Bottleneck Detection, Root Cause Analysis, Time Series Trends, and Machine Learning for High Risk Product Detection.

---

## 📌 Project Overview

This project analyzes a **manufacturing supply chain dataset** with 500 records and 25 features across Indian plants and suppliers. The goal is to identify inefficiencies, detect bottlenecks, and predict high-risk products using data analytics and machine learning.

---

## 🗂️ Dataset Details

| Property | Value |
|---|---|
| File | `manufacturing_supply_chain_data.csv` |
| Rows | 500 |
| Columns | 25 |
| Time Period | January 2023 – November 2023 |
| Domain | Manufacturing Supply Chain (India) |

### 📋 Column Description

| Column | Type | Description |
|---|---|---|
| Product Category | Categorical | Type of product (Raw Material, Semi-Finished, Finished Goods, Spare Parts, Packaging) |
| SKU | Categorical | Unique Stock Keeping Unit identifier |
| Supplier Name | Categorical | Supplier (Tata Steel, JSW Steel, Hindalco, SAIL, Vedanta) |
| Plant Location | Categorical | Manufacturing plant (Katni, Raipur, Nagpur, Bhopal, Indore) |
| Warehouse | Categorical | Storage warehouse (WH-North/South/East/West/Central) |
| Transport Mode | Categorical | Mode of transport (Road, Rail, Air, Courier) |
| Order Priority | Categorical | Priority level (Low, Medium, High, Critical) |
| Order Quantity | Numerical | Number of units ordered |
| Unit Price (Rs.) | Numerical | Price per unit in INR |
| Revenue Generated | Numerical | Total revenue from the order in INR |
| Manufacturing Cost | Numerical | Cost of manufacturing in INR |
| Shipping Cost | Numerical | Cost of shipping in INR |
| Storage Cost | Numerical | Cost of warehousing in INR |
| Stock Level | Numerical | Current inventory stock level |
| Reorder Point | Numerical | Minimum stock level before reorder |
| Lead Time (Days) | Numerical | Days from order placement to delivery |
| Manufacturing Lead Time | Numerical | Days taken for manufacturing |
| Shipping Time (Days) | Numerical | Days taken for shipping |
| Production Volume | Numerical | Total units produced |
| Defect Rate | Numerical | Proportion of defective products (0–1) |
| Inspection Status | Categorical | Quality inspection result (Pass, Fail, Pending) |
| On Time Delivery | Categorical | Whether order was delivered on time (Yes/No) |
| Return Rate | Numerical | Proportion of products returned (0–1) |
| Customer Satisfaction | Numerical | Customer satisfaction score (2.5–5.0) |
| Order Date | DateTime | Date and time of order placement |

---

## 🔍 Analysis Steps

| Step | Description |
|---|---|
| 1️⃣ Data Loading & First Look | Shape, dtypes, missing values, basic statistics |
| 2️⃣ Exploratory Data Analysis | Revenue, production, defect rate by category, supplier, transport |
| 3️⃣ Data Cleaning & Feature Engineering | Derived KPIs — Total Cost, Gross Profit, Profit Margin %, Inventory Turnover, Total Lead Time |
| 4️⃣ Research Questions | 6 business questions answered with visualizations |
| 5️⃣ Bottleneck Detection | Bottleneck Score formula — Supplier × Plant heatmap |
| 6️⃣ Root Cause Analysis | Correlation matrix + Defect Rate deep dive |
| 7️⃣ Time Series Analysis | Monthly trends — Revenue, Orders, Lead Time, Defect Rate, Satisfaction |
| 8️⃣ Machine Learning | Random Forest Classifier — High Risk Product Detection (89% accuracy) |
| 9️⃣ Business Insights | Auto-generated KPI summary + 7 actionable recommendations |

---

## 📊 Charts Generated

| File | Description |
|---|---|
| `01_eda_category_overview.png` | Revenue, Production Volume, Defect Rate by Category |
| `02_eda_supplier_transport.png` | Revenue by Supplier, Shipping Cost by Transport Mode |
| `03_eda_distributions.png` | Lead Time, Defect Rate, Customer Satisfaction distributions |
| `04_research_questions.png` | 6 business research question charts |
| `05_bottleneck_detection.png` | Bottleneck heatmap + Top bottleneck ranking |
| `06_rca_correlation.png` | Full correlation matrix (15 numeric features) |
| `07_rca_defect_deep_dive.png` | Defect Rate by Inspection Status, Transport, vs Satisfaction |
| `08_time_series.png` | 6 monthly trend charts across 2023 |
| `09_ml_model.png` | Confusion Matrix + Feature Importance chart |

---

## ⚙️ Tech Stack

- **Python 3.8+**
- **Pandas** — Data manipulation
- **NumPy** — Numerical operations
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical plots
- **Scikit-Learn** — Machine Learning (Random Forest)

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/Animeshyadav1/manufacturing-supply-chain-analysis.git
cd manufacturing-supply-chain-analysis
```

### 2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 3. Run in Jupyter Notebook
- Open `supply_chain_manufacturing.ipynb`
- Run each cell **top to bottom** in order
- All 9 charts will appear inline

---

## 📁 Repository Structure

```
manufacturing-supply-chain-analysis/
│
├── supply_chain_manufacturing.ipynb   ← Main Jupyter Notebook
├── manufacturing_supply_chain_data.csv ← Dataset (500 rows, 25 columns)
├── README.md                          ← Project documentation
│
└── outputs/
    ├── 01_eda_category_overview.png
    ├── 02_eda_supplier_transport.png
    ├── 03_eda_distributions.png
    ├── 04_research_questions.png
    ├── 05_bottleneck_detection.png
    ├── 06_rca_correlation.png
    ├── 07_rca_defect_deep_dive.png
    ├── 08_time_series.png
    └── 09_ml_model.png
```

---

## 💡 Key Findings

- **Raw Material** is the highest revenue-generating product category
- **SAIL** has the highest average defect rate among all suppliers
- **Nagpur Plant** has the longest average total lead time (43.7 days)
- **11%** of products are flagged as High Risk by the ML model
- **Vedanta** is the best-performing supplier for on-time delivery (76.2%)
- **Random Forest** model achieves **89% accuracy** in detecting high-risk products

---

## 👤 Author

**Animesh Yadav**
- 📧 animeshyadav310@gmail.com
- 💼 [LinkedIn](https://www.linkedin.com/in/animesh-yadav-/)
- 🐙 [GitHub](https://github.com/Animeshyadav1)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
