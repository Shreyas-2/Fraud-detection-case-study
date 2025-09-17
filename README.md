# Credit Card Fraud Detection – Case Study & Dataset Report  

## 📌 Overview  
This repository contains a case study and dataset report on **Credit Card Fraud Detection** in the **Finance and Banking domain**.  
The aim is to explore a publicly available credit card transaction dataset, describe its structure, analyze key metrics, and provide insights for **high-risk transaction detection**.

## 🎯 Case Study  
- **Domain:** Finance and Banking  
- **Case Study:** Fraud Detection and Risk Management  
- **Dataset:** Credit Card Fraud Detection Dataset (Kaggle – ULB Machine Learning Group)  

This dataset is widely used for benchmarking fraud detection and anomaly detection models.  
It contains anonymized credit card transactions where the target label indicates whether a transaction is fraudulent.

## 📂 Dataset Details  
- **Original Size:** 284,807 transactions × 31 features  
- **Subset Used in This Report:** 1,000 transactions × 8 features (for demonstration)  
- **Features (subset):**  
  - `Time` – Seconds elapsed between this and the first transaction  
  - `V1–V5` – Anonymized PCA features  
  - `Amount` – Transaction amount  
  - `Class` – Target label (0 = Non-Fraud, 1 = Fraud)  

## 📊 Key Metrics  
- Fraudulent transactions are extremely rare (~0.6% in this subset)  
- High-value transactions exist but are uncommon  
- PCA features (V1–V5) capture complex behavior of transactions  

## 📝 Sample Records (first 5 rows)  

| Time | V1 | V2 | V3 | V4 | V5 | Amount | Class |
|------|------|------|------|------|------|--------|-------|
| 12810 | 0.49 | -0.67 | -0.23 | 1.57 | -0.46 | 1100.56 | 0 |
| 15276 | -0.13 | -0.46 | 1.46 | -0.22 | 0.54 | 523.44 | 0 |
| 11919 | 0.64 | -0.46 | -0.90 | -1.01 | -0.60 | 1850.12 | 0 |
| 84550 | 1.52 | -0.46 | -0.56 | 0.31 | -0.29 | 984.77 | 0 |
| 13218 | -0.23 | 0.24 | 0.11 | -0.90 | -0.60 | 246.31 | 0 |

*(Full 20-row sample included in the PDF report.)*

## 📈 Charts Included in the Report  
- Fraud vs. Non-Fraud Transaction Distribution  
- Transaction Amount Distribution  

## 🔍 High-Risk Transaction Detection (Insights)  
Criteria used to identify high-risk transactions:
- High Amount (e.g., >90th percentile)  
- Anomalous PCA features (V1–V5 outliers)  
- Multiple transactions in a short time window  
- Low historical frequency for card/user  

## 📑 Report  
The full case study report (PDF) is included in this repository:  
- **[Report.pdf](Report.pdf)**  

## ✅ Conclusion  
This case study demonstrates how to explore a real-world dataset for fraud detection.  
By understanding class imbalance, transaction patterns, and high-risk criteria, financial institutions can better design and train fraud detection systems.

---
