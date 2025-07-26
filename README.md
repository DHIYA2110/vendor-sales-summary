# Vendor-Sales-Summary
Vendor performance analysis using Python, Power BI, and SQL

## Dashboard

[Power BI dashboard](https://drive.google.com/file/d/1Rwdx3EMwJHD_2IxDLvlZ6Z7xy-sfWL6j/view?usp=sharing)

[DASHBOARD PDF](https://drive.google.com/file/d/1c4N_bqLmh0rL4J8pTm9oulegKOOU07H7/view?usp=sharing)

## Dataset

- `vendor_sales_summary.csv` – Final processed dataset for analysis

[LINK](https://drive.google.com/file/d/1Ezu1uxLJZTXoh5iu5s9cLuLy7Xn6Rmup/view?usp=sharing)


#REPORT

[REPORT LINK](https://drive.google.com/file/d/1z5KsJbD5laBcCtfjLOTn1eW0IrTJMEHz/view?usp=drive_link)


# Vendor Sales Summary Analysis

## Business Problem
Business Problem
Effective inventory and sales management are critical for optimizing profitability in the retail and wholesale industry. Companies need to ensure that they are not incurring losses due to inefficient pricing, poor inventory turnover, or vendor dependency. The goal of this analysis is to:
• Identify underperforming brands that require promotional or pricing adjustments.
• Determine top vendors contributing to sales and gross profit.
• Analyze the impact of bulk purchasing on wnit costs.
• Assess inventory turnover to reduce holding costs and improve efficiency.
• Investigate the profitability variance between high-performing and low-performing vendors.


## Project Workflow
1. Data Collection & Integration

Combined multiple datasets: purchases, sales, vendor invoices, purchase prices, and inventory data.

2. Data Cleaning & Preprocessing

Removed inconsistent or irrelevant records (e.g., zero sales quantities, negative profits/margins).

Standardized vendor names and product descriptions.

3. Exploratory Data Analysis (EDA)

Identified outliers in prices, freight costs, and stock turnover.

Assessed vendor contribution and sales performance.

4. Vendor Performance Analysis

Measured Gross Profit, Profit Margin, Stock Turnover, and Sales-to-Purchase Ratios.

Segmented vendors into top performers and low performers.

5. Correlation & Statistical Analysis

Analyzed relationships between pricing, sales, margins, and turnover.

Conducted hypothesis testing to compare profit margins between top-selling and low-selling vendors.

6. Actionable Insights & Recommendations

Derived data-backed strategies for pricing optimization, inventory management, and vendor diversification.


## Key Insights
1.Losses & Zero-Sales Products

Gross profit has a minimum of –52,002, indicating losses on certain products (e.g., sold below cost).

Some products show zero sales, tying up $2.71M in unsold inventory.

2. Vendor Dependency

Top 10 vendors contribute 65.69% of total purchases — over-reliance on a small vendor group increases supply chain risk.

3.Bulk Purchasing Advantage

Bulk orders reduce per-unit costs by ~72%, significantly improving profitability.

4. Profitability Differences Between Vendor Segments

Top vendors: Profit margin ≈ 31.17%

Low-performing vendors: Profit margin ≈ 41.55% (but low sales).

Hypothesis testing confirms statistically significant differences in profitability models.

5.Pricing & Margin Correlations

Weak correlation between purchase price and revenue (–0.012), indicating that pricing changes alone don’t drive sales.

Negative correlation between sales price and profit margin (–0.179), suggesting aggressive pricing cuts into margins.

6. Freight & Logistics Inefficiencies

Freight costs vary widely (0.09 – 257,032), indicating erratic shipping practices or bulk shipment disparities.

7. Stock Turnover Gaps

Stock turnover ranges 0 – 274.5, meaning some products sell very quickly while others stagnate.

## Recommendations
• Re-evaluate pricing for low-sales, high-margin brands to boost sales volume without sacrificing profitability.
• Diversify
• Diversify vendor partnerships to reduce dependency on a few suppliers and mitigate supply chain risks,
• Leverage bulk purchasing advantages to maintain competitive pricing while optimizing inventory management.
• Optimize slow-moving inventory by adjusting purchase quantities, launching clearance sales, or revising storage strategies.
• Enhance marketing and distribution strategies for low-performing vendors to drive higher sales volumes without compromising profit margins.
• By implementing these recommendations, the company can achieve sustainable profitability, mitigate risks, and enhance overall operational efficiency


