# Customer Segmentation using RFM Analysis & K-Means Clustering

## 📌 Overview
This project segments e-commerce customers based on their purchasing behavior 
using the RFM (Recency, Frequency, Monetary) framework combined with K-Means 
clustering. The goal is to help a business identify high-value customers, 
at-risk customers, and design targeted retention/marketing strategies.

## 🎯 Business Problem
Treating all customers the same wastes marketing budget and misses opportunities 
to retain high-value customers. This project identifies distinct customer 
segments so a business can prioritize retention efforts and personalize 
marketing strategies effectively.

## 🛠️ Tools & Skills Used
- **Python** (Pandas, NumPy) — data cleaning & feature engineering
- **Scikit-learn** — StandardScaler, K-Means Clustering, Elbow Method
- **Matplotlib** — data visualization
- **Generative AI (Claude)** — AI-assisted business persona generation

## 📊 Dataset
Online Retail Dataset (UCI Machine Learning Repository) — 500K+ real 
e-commerce transactions from a UK-based online retailer.

## 🔍 Approach
1. **Data Cleaning:** Removed cancelled orders, missing CustomerIDs, and 
   invalid price entries (541,909 → 397,884 valid transaction records)
2. **Feature Engineering:** Calculated Recency, Frequency, and Monetary 
   values per customer
3. **Scaling:** Applied StandardScaler to normalize RFM values before clustering
4. **Clustering:** Used the Elbow Method to determine optimal cluster count 
   (k=4), then applied K-Means clustering
5. **Segmentation & Persona Building:** Labeled clusters into actionable 
   business segments and used AI-assisted analysis to generate personas 
   and marketing recommendations

## 📈 Key Findings
| Segment | Customers | Avg Recency | Avg Frequency | Avg Monetary |
|---|---|---|---|---|
| VIP/Champions | 13 (0.3%) | 7 days | 82.5 orders | ₹127,338 |
| Loyal High-Value | 204 (4.7%) | 15.5 days | 22.3 orders | ₹12,709 |
| Regular/Promising | 3,054 (70.6%) | 43.7 days | 3.7 orders | ₹1,359 |
| At Risk/Lost | 1,067 (24.7%) | 248 days | 1.6 orders | ₹481 |

**Key Insight:** Just 0.3% of customers (VIPs) generate disproportionately 
high revenue, while ~25% of the customer base is at risk of churning — 
highlighting a clear retention priority.

## 💡 Business Recommendations
- **VIP/Champions:** Retain via premium loyalty programs and early product access
- **Loyal High-Value:** Upsell/cross-sell to move them toward VIP status
- **Regular/Promising:** Increase engagement through personalized offers
- **At Risk/Lost:** Launch win-back campaigns with targeted discounts

## 📁 Files
- `customer_segmentation_rfm_kmeans.ipynb` — Full analysis notebook
