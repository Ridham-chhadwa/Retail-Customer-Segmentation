
# Retail Customer Segmentation using RFM and K-Means

## Overview
This project segments retail customers based on purchasing behaviour using the **RFM (Recency, Frequency, Monetary)** model and **K-Means clustering**.  
It helps businesses identify VIP customers, churn risks, and potential growth segments for targeted marketing strategies.

---

## Dataset
**Dataset:** Online Retail II (UCI Repository)

| Variable | Description |
|-----------|-------------|
| InvoiceNo | Unique transaction ID |
| StockCode | Product code |
| Description | Product name |
| Quantity | Items per transaction |
| InvoiceDate | Transaction date |
| UnitPrice | Price per unit |
| CustomerID | Unique customer ID |
| Country | Customer country |

---

## Steps and Methodology

1. **Data Cleaning:**  
   - Removed missing CustomerIDs and cancelled transactions.  
   - Filtered only positive quantities and prices.

2. **Feature Engineering (RFM):**  
   - Recency: Days since last purchase.  
   - Frequency: Number of unique purchases.  
   - Monetary: Total amount spent per customer.

3. **Data Scaling:**  
   - Standardized RFM values for clustering comparability.

4. **Segmentation (K-Means):**  
   - Used the Elbow method to determine optimal K.  
   - Segmented customers into 4 key clusters.

5. **Visualization & Insights:**  
   - Histograms, heatmaps, 3D scatter plots, and revenue share pie chart.  
   - Explained behaviour of each cluster in business terms.

---

## Results

| Cluster | Profile | Key Traits |
|----------|----------|------------|
| 0 | **Champions** | High frequency & monetary, recent buyers |
| 1 | **At Risk** | Long gap since last purchase, low frequency |
| 2 | **Loyal Regulars** | Moderate spenders with consistent engagement |
| 3 | **New Customers** | Recently joined, potential to grow |

Top 20% of customers drive nearly **65% of total revenue**.

---

## Business Impact

This segmentation enables marketing teams to:
- Prioritize high-value customers (loyalty programs).
- Re-engage churn risks via email campaigns.
- Identify cross-sell and upsell opportunities.

---

## Tech Stack
- Python
- pandas, numpy, scikit-learn
- matplotlib, seaborn
- Jupyter Notebook

---

## Author
**Ridham Chhadawa**  
Data & AI Engineer | Sydney, Australia  
[LinkedIn](https://www.linkedin.com/in/ridham-chhadwa-9667a216b/) | [GitHub](https://github.com/ridhamchhadawa)

