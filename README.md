# 🛒 E-Commerce Data Cleaning & Analysis Project

### 🎯 Business Problem & Project Overview
The raw e-commerce dataset (10,000 rows) was heavily corrupted with missing values, inconsistent formatting, and extreme statistical anomalies. These issues prevented accurate revenue reporting and led to biased business insights. My goal was to transform this raw data into a high-integrity asset ready for strategic decision-making.

### 🛠️ Technical Solutions & Workflow
* **Data Auditing & Structural Cleaning:** Standardized all text fields and handled whitespace errors. Converted date features into standard `datetime64[ns]` format using **Python** and **Pandas**.
* **Advanced Missing Value Imputation:** Solved critical data gaps by mathematically reconstructing missing `Quantity` fields ($\text{Revenue} / \text{Unit Price}$) and dropping structurally broken records to ensure consistency.
* **Statistical Outlier Management:** Mitigated the impact of extreme values by applying the **Interquartile Range (IQR)** method to isolate and eliminate 114 revenue outliers (transactions above $26.8k), stabilizing the distribution for unbiased reporting.

### 💡 Key Business Results
* **Data Integrity:** Achieved 100% data cleanliness and reliability for downstream analysis.
* **Strategic Insights:** Identified **Books, Sports, and Home** as the primary revenue drivers.
* **BI Readiness:** Delivered a verified dataset optimized for seamless Power BI Dashboard integration.
