📦# DataCo Global Supply Chain Analytics

End-to-end supply chain, profitability, shipping SLA, and payment fraud analysis built using **Kaggle**, **Google Sheets**, **Fivetran**, **Snowflake**, and **Power BI**.

**Prepared by:** Swati Singhal | Data Analyst

---

## Executive Summary

Fragmented reporting across logistics, pricing, and payment operations can hide margin leakage and delivery bottlenecks. This project analyzes supply chain order records from January 2015 to January 2018 to highlight key operational risks and opportunities:

- **Gross Sales & Net Profit:** $36.78M gross sales and $3.97M net profit (10.78% margin)
- **Shipping SLA Performance:** 54.83% late delivery rate (3.50 actual days vs. 2.93 scheduled days, 0.57 days delay variance)
- **Promotional Discounting:** $3.73M total discounts (10.17% average discount rate)
- **Payment & Fraud Exposure:** $825.93K suspected fraud exposure (2.26% fraud rate)

---

## Data Pipeline

1. **Kaggle:** Sourced raw supply chain order records (January 2015 – January 2018).
2. **Google Sheets:** Cleaned fields, validated structure, and added a `PERIOD_TYPE` filter to separate full-year periods (2015–2017) from partial data (January 2018).
3. **Fivetran → Snowflake:** Loaded cleaned data into Snowflake as the single source of truth.
4. **Power BI:** Built a data model, DAX measures, and a 4-page interactive dashboard.

---

## Key Findings

### 1. Revenue & Margin by Market and Segment
- Europe and LATAM drive major regional revenue, with Consumer leading customer segments over Corporate and Home Office.
- The `PERIOD_TYPE` filter prevents misleading comparisons between full calendar years (2015–2017) and January 2018.

### 2. Shipping Delays & SLA Performance
- Overall late delivery rate is 54.83%, with actual shipping averaging 3.50 days against 2.93 scheduled days.
- First Class and Second Class have high late delivery rates compared to Standard Class.

### 3. Product Departments & Profit Leakage
- Fan Shop and Apparel lead department sales, while categories like Fishing and Cleats stand out on profit.
- Heavy promotional discounting ($3.73M total) reduces net profit margins.

### 4. Payment Methods & Fraud Risk
- Orders span Debit, Transfer, Payment, and Cash channels.
- Suspected fraud accounts for 2.26% of order records ($825.93K exposure), concentrated in Transfer orders.

---

## Recommendations

1. **Improve Delivery SLAs:** Review transit times and capacity for high-delay shipping modes.
2. **Control Discounting:** Set clear limits on promotional discounts in lower-margin categories.
3. **Strengthen Fraud Checks:** Add extra review steps for high-risk Transfer transactions.

---

## Files in This Repository

- `Business Requirements Document - DataCo Supply Chain.pdf`
- `DataCO- Gobal Supply chain ppt.pdf`
- `DataCo Supply Chain Dasboard.pdf`

---

## Connect

- **GitHub:** https://github.com/swatisinghal981

📂- dataco-global-supply-chain-analytics/
├── README.md
├── Business Requirements Document - DataCo Supply Chain.pdf
├── DataCO- Gobal Supply chain ppt.pdf
└── DataCo Supply Chain Dasboard.pdf
