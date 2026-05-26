# 📊 CredPal Consumer Financial Behavior Analysis
[https://public.tableau.com/app/profile/oghenenyerhovwo.omonode2518/viz/CredPal_17618538197580](url)
**Tool:** Tableau | **Dataset:** 10,000 records | **Scope:** 185 Countries · 7 Regions · 12 Consumer Segments

---

## Overview

This project explores consumer financial behavior across global markets using data provided by CredPal — a Buy Now, Pay Later (BNPL) and consumer credit platform. The analysis uncovers patterns in income distribution, monthly expenditure, savings rates, and consumer preferences, with the goal of identifying where credit demand is highest and which consumer segments drive the most financial activity.

The Tableau workbook contains **11 interactive worksheets** and **6 dashboards**, all built from a structured dataset of 10,000 sampled consumers across regions spanning Africa, Asia, Europe, the Americas, and beyond.

---

## Business Questions Explored

- Which regions generate the highest income and expenditure?
- What consumer preferences correlate with the highest spending?
- How do average monthly income and disposable income vary across markets?
- What is the savings rate across different regions and sample groups?
- Which consumer segments should be prioritized for credit product targeting?

---

## Dashboards & Worksheets

### Dashboards
| Dashboard | Focus Area |
|---|---|
| Dashboard 1 | Regional income and expenditure breakdown |
| Dashboard 2 | Consumer preference distribution and spending patterns |
| Dashboard 3 | Savings rate analysis across regions |
| Dashboard 4 | Sample priority vs. financial metrics |
| Summary | High-level KPI overview |
| Summary (2) | Extended summary with segment-level insights |

### Worksheets
- **Avg Disposable Income** — Calculated disposable income per consumer segment
- **Avg Monthly Income By Region** — Regional income comparison
- **Consumer Expenditure** — Monthly spend patterns across consumer types
- **Consumer Preference With The Highest Expenditure** — Identifying highest-spend preference groups
- **Consumer Preferences** — Full distribution of consumer preference categories
- **Highest Consumer Preferences** — Top-ranking preferences by volume
- **Monthly Expenditure** — Time-series and cross-segment expenditure view
- **Region With The Highest Income, Expenditure & Customer Preference** — Multi-metric regional comparison
- **Region With The Highest Income, Expenditure & Savings** — Income vs. savings trade-off by region
- **Relationship Between Income, Expenditure & Savings** — Correlation analysis
- **Savings Rate** — Savings as a percentage of total income across segments

---

## Dataset Schema

| Column | Type | Description |
|---|---|---|
| Region | String | Geographic region (7 unique regions) |
| Country | String | Country of the sampled consumers (~185 countries) |
| Consumer Preference | String | Consumer category/preference segment (12 types) |
| Sample Priority | String | Priority classification of the sample (4 levels) |
| Study Time: Start | Date | Study period start date |
| Study Time: Ends | Date | Study period end date |
| Number of Samples | Integer | Sample size for the record |
| Average Monthly Income ($) | Float | Average income per consumer in the sample |
| Month Expenditure ($) | Float | Average monthly spend per consumer |
| Total Income of Sample Size ($) | Float | Aggregate income across the full sample group |
| Total Expenditure of Sample Size ($) | Float | Aggregate expenditure across the sample group |
| Disposable Income of Sample Size ($) | Float | Aggregate disposable income (income minus expenditure) |

### Calculated Fields
- **Avg Disposable Income** = `Average Monthly Income - Month Expenditure`
- **Savings Rate** = `Disposable Income of Sample Size / Total Income of Sample Size × 100`

---

## Key Insights

- **7 global regions** were analyzed, highlighting stark contrasts in income and expenditure levels across markets.
- **Consumer preferences** vary significantly by region — certain categories consistently drive higher expenditure, making them prime targets for BNPL product offers.
- The **Savings Rate** metric reveals which populations retain the most disposable income, indicating latent credit appetite and risk profile.
- Regions with high income but moderate savings rates represent the sweet spot for credit product penetration.

---

## Tools & Skills Demonstrated

- Tableau Desktop (v2025.2)
- Data extraction and connection via Excel (.xlsx)
- Calculated field creation (DAX-equivalent logic in Tableau)
- Multi-dashboard storytelling
- Geographic mapping with ISO 3166-2 country codes
- Consumer segmentation and behavioral analysis
- Financial KPI design (income, expenditure, savings rate)

---

## File Structure

```
credpal-consumer-financial-analysis/
│
├── CredPal_Analysis.twbx       # Packaged Tableau workbook (includes data extract)
└── README.md
```

> **Note:** The `.twbx` file is a self-contained Tableau packaged workbook. It includes the embedded data extract so no external data connection is required to open and explore the dashboards.

---

## How to Open

1. Download and install [Tableau Public](https://public.tableau.com/en-us/s/download) (free) or Tableau Desktop.
2. Clone this repository or download the `.twbx` file.
3. Double-click `CredPal_Analysis.twbx` to open directly in Tableau.
4. Navigate between dashboards using the tabs at the bottom of the workbook.

---

## Author

**Oghenenyerhovwo Omonode**
Data Analyst | Tableau | SQL | Excel | Power BI

---

*This project was built as part of a data analytics portfolio to demonstrate proficiency in Tableau, consumer financial data analysis, and business intelligence storytelling.*
