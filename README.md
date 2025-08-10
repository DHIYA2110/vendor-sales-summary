## Vendor Sales Summary 

 ## Project Overview
This project analyzes vendor sales performance by integrating and transforming raw sales, purchase, pricing, and freight datasets into a single vendor sales summary table.
The analysis focuses on profitability, inventory efficiency, vendor contributions, and pricing strategies, with actionable business insights and visualizations.

## project Structure
![project_structure](reports/images/project_structure.png)


---

##  Methodology
1. **Data Ingestion** – All raw CSV files are loaded into `inventory.db` using `ingestion_db.py`.
2. **Data Transformation** – `get_vendor_summary.py` merges purchase, sales, price, and freight data to create a **vendor_sales_summary** table.
3. **Data Cleaning** – Missing values filled, data types fixed, and calculated metrics added:
   - `GrossProfit`
   - `ProfitMargin`
   - `StockTurnover`
   - `SalesToPurchaseRatio`
4. **Exploratory Data Analysis** – Performed in `vendor_performance_analysis.ipynb`.
5. **Visualization & Insights** – Created impactful graphs to communicate business findings.

---

##  Key Insights & Visuals

### **1️⃣ Vendor Contribution & Market Share**
![Pareto Vendor Contribution](reports/images/pareto_vendor_contribution.png)
-65.69% of purchases come from the top 10 vendors.
-Heavy vendor dependency introduces supply chain risk — diversification recommended.
- **Top 10 vendors** account for a significant percentage of total purchases, indicating a **high vendor concentration** and potential **supply chain risk**.
- Some vendors have **dominant purchase shares but lower sales performance**, signaling possible **inventory overstock** or **slow-moving goods**.

---

### **2️⃣ Sales Performance Leaders**
![Top Vendors by Sales](reports/images/top_10_vendors_by_sales.png)
![Top Brands by Sales](reports/images/top_btrands_by_sales.png)
-198 brands have low sales but high margins.
-Opportunity to boost volumes without sacrificing profitability.
- **Top Vendors by Sales** clearly show a **core group driving revenue**, making them priority partners for **marketing and promotional investments**.
- **Top Brands by Sales** reveal **customer preferences**, helping guide **inventory planning** and **brand-focused promotions**.


### **3️⃣ Profitability Analysis**

![Profit Margin Confidence Interval](reports/images/profit_margin_confidence_interval.png)
- **Profit Margin Distribution** shows strong margins for certain vendors, while others have **thin or negative margins**, potentially due to **discount-heavy strategies** or **pricing misalignment**.
- **Confidence interval analysis** indicates a **clear performance gap** between top and bottom vendors, suggesting that **margin optimization** could boost overall profitability.
- **Strategic implication**: Prioritize partnerships with high-margin vendors and adjust pricing for low-margin brands.

---

### **4️⃣ Pricing & Promotional Opportunities**
![Brands for Promotional Pricing Adjustment](reports/images/brands_for_promotional_pricing_adj.png)
- The **Promotional Pricing Adjustment scatter plot** identifies brands where **price changes** could stimulate demand without hurting profitability.
- **Strategic implication**: Run targeted price tests for low-selling, high-margin brands to increase turnover.

---

### **5️⃣ Purchase Efficiency & Cost Optimization**
![Bulk Purchase vs Unit Price](reports/images/bulk_purchase_vs_unit_price.png)
-Bulk orders lower unit cost by ~72% ($10.78 vs. smaller-order prices).
-Encourages larger vendor orders while maintaining margins.
- **Bulk Purchase Impact on Unit Price** confirms that **larger purchase volumes** often secure **lower per-unit costs**, validating bulk procurement strategies.
- **Strategic implication**: Increase bulk orders for fast-moving products to maximize cost efficiency.

---


### **6️⃣  Operational Metrics from Vendor Summary**
-$2.71M capital locked in slow-moving inventory.
-Key low-turnover vendors:

 ALISA CARR BEVERAGES (0.615x turnover)
 HIGHLAND WINE MERCHANTS LLC (0.708x turnover)
 PARK STREET IMPORTS LLC (0.751x turnover)
- **Stock Turnover** analysis shows certain vendors have **slower-moving stock**, increasing **holding costs**.
- **Sales-to-Purchase Ratio** highlights inefficiencies in converting purchases into sales for some vendors.


##  Future Improvements
- Automate data ingestion via scheduled ETL pipelines.
- Add forecasting models to predict vendor performance.
- Integrate dashboarding tools (Power BI / Tableau) for real-time reporting.
- Enhance data quality checks to handle missing or inconsistent records.

---

##  How to Run the Project
```bash
# 1. Clone repository
git clone https://github.com/your-username/vendor-sales-summary.git
cd vendor-sales-summary

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run ingestion script to load data into database
python ingestion_db.py

# 4. Generate vendor sales summary table
python get_vendor_summary.py

# 5. Open Jupyter Notebook for analysis
jupyter notebook notebooks/vendor_performance_analysis.ipynb
