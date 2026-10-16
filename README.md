# Block-Production-Sales-Python-Analysis
Python (pandas) analysis of a block-moulding business's production and sales performance from 2021 to 2025 — originally built as an Excel dashboard with supporting SPSS/STATA statistical work, rebuilt, validated and extended here in Python.

# 🧱 Block Production & Sales Performance Analysis

📊 **A Python-based business analytics project | December 2021 – December 2025**

This project examines production, sales, profitability, customer behaviour, and credit risk for a block-moulding business. The analysis was first developed through Excel dashboards and supporting SPSS/STATA statistical work, then rebuilt, cross-checked, and extended in Python.

> **Business question:** What actually drives profit—and what should the business monitor to make better production, pricing, cost-control, and customer decisions?

## 🎯 Project at a Glance

* **Business:** Concrete block production and sales (6-inch, 7-inch, and 9-inch blocks)
* **Period covered:** December 2021 to December 2025
* **Analytical workflow:** Data preparation → exploratory analysis → KPI and trend analysis → statistical modelling → validation → business recommendations
* **Tools:** Python, pandas, NumPy, Matplotlib, Seaborn, SciPy, statsmodels, Excel, SPSS/STATA, and Power BI

## 💡 Executive Highlights

* 💰 **₦3,178,565 total profit** from **₦18,633,540 revenue**, representing a **17.1% profit margin**.
* 🧱 **45,879 blocks produced** and **43,230 blocks sold**—a reported **94.2% sell-through**.
* 📈 Production was strongly associated with sales, cost, and revenue (**r ≈ 0.82–0.85**), but its relationship with profit was very weak (**r = 0.09**, not statistically significant). **Higher output alone did not guarantee higher profit.**
* 🧮 The profit-driver model identified sales volume and cost as important factors. The reported estimates were approximately **₦221 additional monthly profit per additional block sold** and **₦0.63 lower profit per additional ₦1 of cost**. Both were statistically significant (**p < 0.001**); model **R² = 0.49**. A robustness check confirmed the findings were not driven solely by product mix.
* 🗓️ Revenue did not show a statistically significant time trend (**p = 0.33**). Production declined by approximately **31 blocks per month** (**p = 0.004**) during a period of reported operational disruption; sales were supported by existing stock.
* 🤝 **40% of customers were repeat buyers**, accounting for **82% of revenue**—a concentrated and valuable customer relationship base.
* 🧾 The reported cost mix was **70.5% variable** and **29.5% fixed**. Sand and cement represented roughly two-thirds of total cost. Cost per block increased from **₦148.8 in 2021** to **₦546.7 in 2025**.
* 🛡️ Bad debt represented **0.99% of billed amount overall**. Its relationship with revenue was weak (**r = 0.37**) and not statistically significant in the reported analysis.

## 🧪 Analytical Approach

1. **Data preparation and quality checks** — standardized field names, reviewed dates and derived calendar fields from the date column, and documented source-data issues.
2. **Exploratory and descriptive analysis** — production and sales patterns, product performance, cost composition, customer behaviour, and business KPIs.
3. **Statistical analysis** — correlation analysis and OLS regression to examine profit drivers, revenue drivers, and time trends; included a product-mix robustness check.
4. **Cross-tool validation** — compared Python results with the earlier Excel and SPSS/STATA work, documenting matches and discrepancies.
5. **Business-focused extensions** — quarterly summaries, exported analytical tables, and product-filtered sales breakdowns.

### ⚠️ Data Handling Notes

* Blank production values were treated as missing where appropriate—not automatically replaced with zero. Any calculation-specific treatment is documented in the notebook.
* Two sales dates recorded as 2014 were corrected to 2024 after review.
* The earlier customer-value pivot excluded two customers whose sales were fully recorded as bad debt, understating quantity sold by 63 blocks.
* One month's blank total cost was derived from its single recorded cost component.
* These are observational business-record analyses. Regression estimates describe associations in the available records; they should not be interpreted as proof of causation.

## ✅ Validation Against Earlier Analysis

The Python workflow was cross-checked against the original report. **Nine of 11 checked figures matched exactly**, including the reported correlation coefficients, cost-per-block progression, the 51% price increase from 2023 to 2024, and both regression R² values. The notebook documents the comparison and two small narrative corrections.

## 📂 Repository Structure

```text
Block-Production-Sales-Python-Analysis/
├── Block_Production_Analysis.ipynb        # Python analysis notebook
├── README.md                              # Project overview and findings
├── requirements.txt                       # Python dependencies
└── data/
    ├── Block_Production_Sales_Source.xlsx # Original business workbook
    └── README.md                          # Source-data notes
```

## 📌 Main Deliverables

* 📓 Python notebook covering data preparation, analysis, validation, and extensions
* 📊 Reproduction of the original dashboard's analytical themes: Executive Overview, Profitability, Production & Demand, and Risk & Customer
* 📄 Executive summary report (available as a separate PDF)
* 🗃️ Original source workbook, included for transparency and reproducibility

## 🔍 What This Analysis Suggests the Business Should Monitor

* **Profit per block and cost per block**—not production volume alone
* **Sales volume and realized selling price** alongside production output
* **Sand and cement costs** as major cost-control priorities
* **Repeat-customer revenue concentration** and customer retention
* **Production interruptions and inventory drawdown** when sales continue despite lower output
* **Bad-debt exposure** by customer, while avoiding conclusions unsupported by the limited statistical relationship

## 👤 Author

**Gafar Olajide** | Data Analyst

🔗 GitHub: https://github.com/Gafar-olajide
