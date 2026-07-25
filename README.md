# 📊 Financial Sales Analysis Dashboard | Power BI + Excel + SQL

**Analyzing $118.7M in sales across 5 segments, 5 countries, and 6 products to find out where the business is actually making money — and where it's quietly losing it.**

---

## 📌 Business Problem

Leadership had transaction-level sales data (product, country, customer segment, discount band, units, revenue, cost, profit) but no consolidated view to answer:

- Which products and segments actually drive revenue *and* profit — not just volume?
- Which countries are strongest, and where is margin being left on the table?
- Is the discounting strategy helping or hurting profitability?
- Is the business growing, and where should focus shift next?

Raw transaction rows can't answer "should we cut the Enterprise segment or double down on Government?" — that requires aggregation, segmentation, and a dashboard stakeholders can filter themselves.

---

## 🎯 What I Did

1. Loaded and modeled 700 sales transaction records (segment, country, product, discount band, sales, gross sales, discounts, COGS, profit, units, date) into MySQL.
2. Wrote SQL queries to aggregate sales, profit, and margin by segment, product, country, discount band, and month.
3. Built a Power BI dashboard (Sales Analytics + Profit & Quantity views) with DAX measures, Power Query cleaning, and interactive filters/drill-downs.

---

## 📊 Impact — The Numbers

*(Computed directly from the transaction dataset)*

| KPI | Value |
|---|---|
| **Total Sales** | **$118.7M** |
| **Total Gross Sales** | $127.9M |
| **Total Discounts Given** | $9.2M |
| **Total Profit** | **$16.9M** |
| **Overall Profit Margin** | **14.2%** |
| **Total Units Sold** | 1,125,806 |

### The headline finding: not every segment that sells the most, profits the most

| Segment | Sales Share | Profit Margin | Verdict |
|---|---|---|---|
| **Government** | 44.2% of sales | **21.7%** | Biggest *and* one of the most profitable — clear priority |
| **Small Business** | 35.7% of sales | 9.8% | High volume, thin margin |
| **Enterprise** | 16.5% of sales | **-3.1% (a loss)** | ⚠️ **Losing money** despite being the #3 segment by revenue |
| Midmarket | 2.0% of sales | 27.7% | Small but highly profitable |
| Channel Partners | 1.5% of sales | **73.1%** | Tiny volume, by far the best margin per dollar sold |

**This is the number that matters most in the whole dataset: the Enterprise segment is sales-positive but profit-negative.** It generates real revenue but actually loses money once cost of goods is accounted for — something a "total sales" view alone would never surface, and something the original project summary didn't call out.

### Other findings
- **Paseo is the top product by both sales ($33.0M) and profit ($4.8M)** — but Amarilla has the *highest margin* of any product (15.9%), ahead of Paseo (14.5%).
- **Country performance is fairly balanced** (US, Canada, France, Germany, Mexico all in the $21M–$25M sales range), but **France and Germany carry the best margins (~15.5–15.7%)** while the US has the lowest (12.0%) despite the highest sales.
- **Discounting is eroding profit disproportionately:** the "High" discount band generated similar sales to the "Medium" band ($37.4M vs $38.8M) but $5.3M in discounts vs. $3.0M — and ends up with the lowest profit of the three bands ($3.4M vs. $5.6M). Heavy discounting is not paying for itself here.
- **Sales grew ~16.5% year over year on a like-for-like monthly basis** (2013 data only covers Sep–Dec, so raw totals aren't comparable — monthly averages are: ~$6.6M/month in 2013 vs. ~$7.7M/month in 2014).

---

## 🧭 How This Drives Business Decisions

| Business Question | Dashboard Answer | Decision It Enables |
|---|---|---|
| Should we keep investing in Enterprise the way we sell to Government? | Enterprise sells well but loses money (-3.1% margin) | Pricing, cost-to-serve, or discount policy review specifically for Enterprise accounts |
| Where should sales leadership double down? | Government = 44% of sales at 21.7% margin | Protect and grow Government relationships as the core profit engine |
| Is our discount strategy working? | High discount band has the worst profit of the three bands | Cap or restructure deep discounting; it's not converting to proportional profit |
| Which product to feature in high-margin campaigns? | Amarilla has the best margin, Paseo the best volume | Bundle/promote Amarilla where margin matters, lead with Paseo where volume matters |
| Which country team is most efficient? | Germany/France beat the US on margin despite similar sales | Study what Germany/France are doing differently (pricing, discount discipline) and apply it in the US market |

---

## 🛠 Tools & Technologies
Power BI Desktop · Power Query · DAX · MySQL · Data Modeling · Data Visualization

## 📂 Repository Structure
```
financial_sales_analysis_excel_sql_powerbi/
│
├── README.md
├── Financial_Sample_MySQL.csv                          # 700 transaction records
├── Financial Sales Analysis - SQL Queries.docx         # SQL queries used
├── Finacial_Sales_Analysis_Report (Power BI).pbix       # Power BI dashboard
└── Finacial_Sales_Analysis_Report (Power BI).pdf        # Dashboard export
```

## 📈 Skills Demonstrated
SQL · Data Cleaning & Transformation (Power Query) · Data Modeling · DAX Measures · Profitability Analysis · KPI Reporting · Business Storytelling · Data Visualization

---

## Dashboard Preview
<img width="684" height="400" alt="image" src="https://github.com/user-attachments/assets/8a9dcadc-281e-4446-ae9a-c0aaded76bb4" />
<img width="671" height="388" alt="image" src="https://github.com/user-attachments/assets/ce79f9ea-69f6-4850-9642-ccad506b361d" />
<img width="673" height="394" alt="image" src="https://github.com/user-attachments/assets/245ad692-99e3-4a08-84b9-a0a7ca0c5986" />



# 👨‍💻 About Me

**Prateek Gupta**

Data Analyst with hands-on experience in:

- SQL
- Excel
- Power BI
- Data Visualization
- Financial Analytics
- Healthcare Analytics

📧 Email: prateekgupta545@gmail.com

💼 LinkedIn: https://linkedin.com/in/prateek-k-gupta

🐙 GitHub: https://github.com/Prateekgupta-08

---

# ⭐ If you found this project helpful

Please consider giving it a ⭐ on GitHub!



