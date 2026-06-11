# 🛒 E-Commerce Data Cleaning & Analysis Project

### 🎯 Project Overview
Transformed a raw, corrupted e-commerce dataset (10,000 rows) into a highly reliable, structured asset ready for strategic business intelligence, ensuring 100% data integrity.

### 🛠️ Technical Workflow & Solutions
* **Data Auditing & Structural Cleaning:** Standardized all text fields (lowercasing and removing structural whitespace formatting errors). Converted date features into standard datetime64[ns] format.
* **Logical Missing Value Imputation:** Resolved critical null values mathematically by reconstructing missing Quantity fields ($\text{Revenue} / \text{Unit Price}$), dropping broken order profiles (Order_ID), and imputing categorical fields.
* **Statistical Outlier Management:** Used the Interquartile Range (IQR) method to isolate and filter out 114 extreme anomaly transactions (above $\$26,812.5$), stabilizing data distribution for unbiased statistical reporting.

### 💡 Key Business Insights
* Identified **Books, Sports, and Home** categories as the primary revenue drivers for the business.
* Delivered a verified, clean dataset (`ecommerce_sales_final_clean.csv`) optimized for seamless Power BI Dashboard integration.
