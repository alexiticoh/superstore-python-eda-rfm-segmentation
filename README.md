# Superstore Customer Segmentation & Statistical EDA (Python)

## 📌 Business Overview
Exploratory Data Analysis (EDA) and unsupervised rule-based customer segmentation (RFM Model) applied to 4 years of retail transactional data. The objective is to statistically quantify the impact of promotional discounts on profit erosion and classify the customer base into actionable commercial segments.

## ⚙️ Tech Stack & Libraries
* **Language:** Python 3.x
* **Core Libraries:** `pandas`, `numpy` (data manipulation and vectorization)
* **Statistical Visualization:** `seaborn`, `matplotlib`
* **Techniques:** Pearson Correlation Heatmap, Quantile Binning (`pd.qcut`), RFM Segmentation Algorithm

## 🔍 Key Findings & Statistical Insights

### 1. Statistical Proof of Margin Destruction (Heatmap & Binning)
* **Correlation:** Pearson coefficient between `Discount` and `Margin_%` is strongly negative (**~ -0.50**), confirming that aggressive price cuts do not drive profitable volume.
* **Critical Threshold:** Transactions with discounts exceeding **20%** consistently yield negative mean profits, with the `>50%` tier generating severe cash drains.

### 2. RFM Customer Segmentation Breakdown (793 Unique Accounts)
The customer base was segmented based on Recency (last purchase date), Frequency (order count), and Monetary value (total spend):

| Customer Segment | Strategy & Actionable Recommendation |
| :--- | :--- |
| **Champions** | High spend, high frequency, recent purchases. Enroll in VIP loyalty tiers and upsell premium lines. |
| **Loyal Customers** | Consistent purchase cadence. Offer personalized product bundles with strict 0-10% discount caps. |
| **At Risk** | High historical spenders with long inactivity (>180 days). Trigger re-engagement campaigns before total churn. |
| **Hibernating / Lost** | Low recency and low frequency. Exclude from paid marketing campaigns to minimize acquisition waste. |

## 🔗 The End-to-End Superstore Analytics Suite
This project completes the three-tier analytics portfolio:
1. 📊 [Interactive Executive Dashboard (Power BI)](https://github.com/alexiticoh/superstore-sales-operations-dashboard)
2. 🗄️ [Relational Database Analysis & Logistics SLA (SQL)](https://github.com/alexiticoh/superstore-sql-business-analytics)
3. 🐍 [Statistical EDA & RFM Segmentation (Python)](https://github.com/alexiticoh/superstore-python-eda-rfm-segmentation)
