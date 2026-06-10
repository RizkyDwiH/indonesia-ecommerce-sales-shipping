# Indonesia E-Commerce Sales & Logistics Analytics

This project analyzes **20,848 e-commerce transactions** across **34 Indonesian provinces** over a **24-month period (December 2023 – November 2025)**.

Using **Python, statistical testing, machine learning, and Tableau**, the analysis uncovers insights related to customer payment behavior, order cancellations, logistics performance, revenue trends, and regional segmentation.

The objective is to help e-commerce businesses improve revenue, reduce cancellations, and optimize logistics operations through data-driven decision making.


## Business Objective

Help e-commerce stakeholders better understand customer purchasing behavior and operational performance in order to:

- Increase digital payment adoption
- Reduce order cancellation rates
- Identify high-risk and high-performing provinces
- Optimize logistics and shipping strategies
- Improve revenue through targeted business initiatives


## Dataset Overview

| Metric | Value |
|---------|---------|
| Total Transactions | 20,848 |
| Analysis Period | Dec 2023 – Nov 2025 |
| Provinces Covered | 34 |
| Cancellation Rate | 14.77% |
| Payment Methods | COD, ShopeePay, Transfer Bank, SeaBank, ShopeePayLater |
| Features Created | Time-based, Payment Group, Cancellation Flag, Log Features |


## Tools & Technologies

| Category | Tools |
|-----------|--------|
| Data Processing | Python, Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn |
| Statistical Analysis | SciPy |
| Machine Learning | Scikit-Learn (K-Means Clustering) |
| Dashboard Development | Tableau Public |
| Environment | Jupyter Notebook |


## Analytical Workflow

### 1. Data Cleaning & Preprocessing
- Datetime conversion
- Missing value handling
- Numeric data cleaning
- Cancellation flag creation

### 2. Feature Engineering
- Payment segmentation (Digital / COD / Other)
- Time-based features (Hour, Month, Year, DayOfWeek)
- Log transformations
- Discount indicators

### 3. Statistical Analysis
- A/B Testing (Digital Payment vs COD)
- T-Test
- Cohen's d Effect Size
- Correlation Analysis

### 4. Customer & Regional Segmentation
- Province-level aggregation
- K-Means Clustering
- Cluster profiling

### 5. Business Intelligence Dashboard
- Sales Performance
- Payment Analysis
- Province Analysis
- Logistics & Cancellation Insights


## Key Findings

### Payment Method Insight
- Digital payment users spend **80.7% more** than COD users.
- Result is statistically significant (**p < 0.001**).
- Despite this, **64% of orders still use COD**, indicating a major growth opportunity for digital payment adoption.

### Cancellation Insight
- Overall cancellation rate: **14.77%**
- Highest cancellation provinces:
  - Sulawesi Tengah (35.7%)
  - Sulawesi Utara (34.1%)
  - Kalimantan Timur (30.8%)

### Logistics Insight
- Higher-risk provinces are concentrated in Eastern Indonesia.
- Shipping performance varies significantly across provinces.
- JNE Trucking (JTR) generated the highest average order value among shipping methods.


### Peak Order Hours

- Peak transaction hours: **20:00 (8 PM)**, **11:00 AM**, and **12:00 PM**
- The highest order volume occurs during **evening shopping hours (20:00)**
- Midday periods (11:00–12:00) also show strong purchasing activity

**Business Implication:**  
Promotions, advertising campaigns, and operational resources should be optimized around peak purchasing periods (11:00–20:00) to improve conversion rates and customer experience.

### Province Segmentation
Four distinct province segments were identified through K-Means clustering:

| Cluster | Characteristics |
|----------|----------------|
| Cluster 0 | Premium Customers, High Shipping Cost, Moderate Risk |
| Cluster 1 | Standard Performance |
| Cluster 2 | Best Performer (Highest Revenue, Lowest Cancellation) |
| Cluster 3 | High-Risk Provinces |


## Business Recommendations

### 1. Increase Digital Payment Adoption
Launch promotional campaigns such as:

- Cashback for ShopeePay
- Digital payment discounts
- Loyalty rewards

### 2. Reduce Cancellation Risk
Focus operational improvements in:

- Sulawesi Tengah
- Sulawesi Utara
- Kalimantan Timur

### 3. Optimize Logistics Strategy
- Prioritize reliable shipping partners in high-risk provinces.
- Promote premium shipping services for high-value transactions.

### 4. Province-Based Strategy
Develop customized marketing and operational strategies for each province cluster.


## Estimated Business Impact

| Initiative | Potential Impact |
|------------|-----------------|
| Reduce cancellation by 25% | Rp39M – Rp52M savings |
| Convert 10% COD users to Digital Payment | Rp85M – Rp110M additional revenue |


## Tableau Dashboard

The interactive dashboard includes:

- Daily Revenue Trend
- Monthly Revenue Trend
- Province Performance Analysis
- Payment Method Analysis
- Shipping Method Analysis
- Hourly Order Distribution
- Order Status & Cancellation Analysis


## Project Structure

```text
├── notebooks/
│   └── ecommerce_analysis.ipynb
│
├── data/
│   ├── raw_data.csv
│   ├── tableau_daily_sales.csv
│   ├── tableau_monthly_trends.csv
│   ├── tableau_payment_analysis.csv
│   ├── tableau_province_analysis.csv
│   ├── tableau_shipping_analysis.csv
│   ├── tableau_hourly_patterns.csv
│   └── tableau_order_status.csv
│
├── dashboard/
│   └── tableau_dashboard.twb
│
├── images/
│   └── dashboard_preview.png
│
└── README.md
