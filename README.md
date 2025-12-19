# ESG Performance Analysis & Financial Data Insights

## Project Overview
This project analyzes **Environmental, Social, and Governance (ESG)** performance of companies and studies how ESG-related stability aligns with key **financial indicators**.  
The goal is to understand **long-term sustainability and risk**, not short-term profit prediction.

This is an end-to-end **data analysis project** implemented using **Python**.

---

## Problem Statement
ESG metrics are widely used to evaluate company responsibility and sustainability, but they are often misunderstood as indicators of short-term financial performance.

**This project answers:**
- Are companies with strong ESG performance more stable in the long run?
- Does good ESG automatically mean better financial results?

---

## Dataset
- Source: Kaggle (Company ESG & Financial Performance Dataset)
- Type: Real-world, company-level, multi-year data

### ESG Features
- ESG_Environmental
- ESG_Social
- ESG_Governance
- ESG_Overall (partially missing)

### Financial Features
- Revenue
- ProfitMargin
- MarketCap
- GrowthRate

Each row represents a company’s performance in a given year.

---

## Approach

### 1. Data Cleaning & Validation
- Inspected schema and data types
- Identified missing values in ESG_Overall
- Ensured ESG scores were within valid ranges
- Removed duplicate records

---

### 2. ESG Score Calculation
Since ESG_Overall had missing values, a new ESG score was calculated:


The calculated score closely matched ESG_Overall where available, validating the scoring logic.

---

### 3. ESG Risk Classification
Companies were categorized into ESG risk groups:

| ESG Score Range | Risk Category |
|---------------|--------------|
| < 40 | High Risk |
| 40–70 | Medium Risk |
| > 70 | Low Risk |

This made ESG insights more interpretable from a business perspective.

---

### 4. Analysis & Insights
- Correlation analysis showed **weak relationships** between ESG scores and short-term financial metrics
- ESG does not strongly impact short-term profit or growth
- However, when grouped by ESG risk level:

**Low ESG Risk companies showed:**
- Higher average revenue
- Larger market capitalization
- Better profit margins
- Higher growth rates

---

## Key Takeaway
> ESG performance is best interpreted as a **long-term stability and risk indicator**, not a predictor of short-term financial returns.

---

## Tools & Technologies
- Python
- Pandas, NumPy
- Jupyter Notebook
- Matplotlib / Seaborn (analysis visuals)

---

## Limitations & Future Scope
- Industry-level differences not isolated
- Long-term stock return analysis not included
- Future work could include dashboards using Power BI or Tableau

---

## Author
**Snehith Reddy Jaggari**
