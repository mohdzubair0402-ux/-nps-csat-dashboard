# NPS & CSAT Customer Feedback Dashboard — Power BI

An interactive Power BI dashboard analyzing 500 customer survey responses to track Net Promoter Score (NPS) and Customer Satisfaction (CSAT) across regions, product categories, and support channels — with drill-through root-cause analysis of detractor feedback.

## Business Problem

Customer support and sales teams were collecting satisfaction survey data across multiple channels (Chat, Email, Phone, In-Store) but had no centralized way to track sentiment trends, compare performance across regions and product lines, or identify *why* customers were becoming detractors. This dashboard consolidates that data into a single interactive view for stakeholders to monitor and act on.

## Key Metrics

| Metric | Value |
|---|---|
| Total Responses | 500 |
| Avg CSAT | 3.65 / 5 |
| NPS % | 12.60% |
| Promoters | 229 (45.8%) |
| Passives | 105 (21.0%) |
| Detractors | 166 (33.2%) |

## Dashboard Screenshots

### Overview
![Overview](https://github.com/mohdzubair0402-ux/-nps-csat-dashboard/blob/main/screenshots/01-overview.png)
Total responses, Avg CSAT, and NPS% at a glance, with slicers for Region, Product Category, and Month. The Promoters/Passives/Detractors breakdown and a monthly NPS% trend line sit alongside a regional NPS comparison.

### CSAT by Product Category
![CSAT by Category]( https://github.com/mohdzubair0402-ux/-nps-csat-dashboard/blob/main/screenshots/02-csat-by-category.png)
Average CSAT broken down by product line, plus a detailed Detractor/Passive/Promoter count table per category.

### Detractor Root-Cause Analysis
![Detractor Analysis](https://github.com/mohdzubair0402-ux/-nps-csat-dashboard/blob/main/screenshots/03-detractor-analysis.png)
Drill-through view showing Detractor counts by Issue Type, with a filterable detail table of individual complaints (e.g., billing errors) and their exact CSAT scores.

## Key Insights

- **Overall NPS of 12.60% signals room for improvement.** With a third of respondents (33.2%) classified as Detractors, the dashboard was built specifically to help leadership pinpoint *why* — not just track the score.
- **Desktop leads on satisfaction (4.11 avg CSAT), while Peripherals (3.39) and Software MS365 (3.48) lag behind** — suggesting the after-sales experience for smaller accessory purchases and subscription software may need attention.
- **Sales Experience is the single largest driver of detractors (50 responses)** — ahead of Tech Support (34), Product Defects (32), and Billing Errors (25) — pointing to the sales process itself, not just the product, as a key area for improvement.
- **Billing Error complaints cluster around three specific issues:** customers charged twice for warranty coverage, refunds not processed, and incorrect pricing applied at checkout. These are operational/process fixes rather than product issues, and relatively quick wins.
- **NPS% swings significantly by month**, dipping into negative territory in February before peaking above 50% in November — worth investigating against seasonal promotions, staffing, or product launches.
- **Regional NPS varies widely**, with the Middle East and APAC scoring highest and Europe scoring lowest, suggesting region-specific follow-up may be more effective than a one-size-fits-all response plan.

## Tools & Techniques

- **Power BI Desktop**: report building, data modeling, interactive slicers
- **DAX measures**: NPS % (Promoters − Detractors), CSAT averages, Promoter/Passive/Detractor classification and counts
- **Drill-through**: Issue Type → Detractor detail table for root-cause investigation
- **Visuals used**: KPI cards, donut chart, line chart, horizontal bar charts, matrix table with conditional formatting

## Files in this Repo

| File | Description |
|---|---|
| `dashboard/NPS_CSAT_Dashboard.pbix` | Power BI source file (requires [Power BI Desktop](https://www.microsoft.com/en-us/power-platform/products/power-bi/downloads), free) |
| `data/survey_data_raw.xlsx` | Raw survey response dataset used to build the model |
| `exports/NPS_CSAT_Dashboard.pdf` | Static PDF export for quick preview without opening Power BI |

## How to Use

1. Download `NPS_CSAT_Dashboard.pbix`
2. Open in Power BI Desktop (free download from Microsoft)
3. Use the Region, Product Category, and Month slicers to filter the view
4. Click into any Issue Type bar on the detractor chart to drill through to individual complaint detail

---
**Author:** Mohd Zubair Ahmed | [LinkedIn](https://linkedin.com/in/mohd-zubair-ahmed-508996263)
