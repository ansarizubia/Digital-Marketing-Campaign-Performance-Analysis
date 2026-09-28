# Digital Marketing Campaign Performance Analysis

Excel + Power BI project | Author: Zubia Ansari | [GitHub](https://github.com/ansarizubia)

## Business problem

A D2C fashion & lifestyle brand runs paid and owned marketing campaigns across six channels and seven Indian metro regions. Marketing spend has grown quarter over quarter, but the team has no single view of which channels, regions, and campaigns actually convert that spend into revenue. Budget allocation decisions are currently made on gut feel rather than performance data.

## Objective

- Consolidate and clean a raw multi-source campaign export
- Calculate standard marketing KPIs (CTR, conversion rate, CPC, CPA, ROAS) at the record level
- Identify which channels, regions, devices, and campaigns deliver the best return on ad spend
- Build an interactive Excel dashboard and a companion Power BI report for ongoing tracking
- Turn the analysis into budget-reallocation recommendations for the next quarter

## Dataset

- 620 cleaned records, weekly grain, July 2025 to May 2026
- One row = one campaign x channel x region x device combination, for one week
- `Raw_Data` (inside the workbook) is the untouched export and contains duplicate rows, inconsistent text casing, mixed date formats, missing values, and a few impossible values (such as clicks exceeding impressions)
- `Cleaned_Marketing_Data.csv` in this repo is the cleaned dataset, ready to import into Power BI

### Tools Used:

**Excel**
- Data cleaning equivalent to Power Query (duplicate removal, text standardisation, date parsing, error correction, missing-value handling)
- Formulas: SUMIFS,PIVOTTABLE,AVERAGEIFS-style aggregation, INDEX/MATCH, IFERROR, RANK, TEXT
- Excel Tables with structured formatting and filters
- Conditional formatting (color scales, rule-based highlighting)
- Data validation dropdown driving a live filtered dashboard
- Named ranges
- Native charts (bar, line) built from formula-driven summary tables

**Power BI**
- Data import and modelling from the cleaned CSV
- Interactive report with slicers and cross-filtering

### Key findings

- Email Marketing returns the highest ROAS (return on ad spend) at roughly 37x, on the smallest media spend share
- Google Ads produces the highest single-channel revenue and conversion volume
- Instagram Ads and Facebook Ads carry the largest combined spend but the lowest ROAS among paid channels (around 6x)
- Diwali Mega Sale is the strongest-performing campaign at close to 15x ROAS, with festive-season campaigns outperforming clearance-style campaigns
- Mobile drives the large majority of spend and conversions

Full findings and recommendations are in the `Insights` sheet of the workbook.

## How to explore this project

1. Open the Excel workbook and start on the `README` sheet for the data dictionary
2. Look at `Raw_Data` to see the data quality issues, then `Cleaned_Data` to see the fix
3. Check `Analysis` for the formula-driven summary tables
4. Use the `Dashboard` sheet's channel filter to explore KPIs interactively
5. Follow `PowerBI_Dashboard_Guide.md` to build the Power BI companion report from `Cleaned_Marketing_Data.csv`

### Author
**Zubia Ansari** - Data and BI Analyst
LinkedIn | GitHub
