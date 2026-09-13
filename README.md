# DeltaTech B.V. — H1 2024 Financial Performance Dashboard

An Excel-based financial analysis project built to turn six months of fragmented sales and cost data into a clear management view of revenue, margins, product performance, regional performance, and practical business actions.

> **Portfolio project:** The workbook is presented as a business case study for analytical and reporting purposes. It is not intended to represent audited company accounts.

## What this project does

The original data is spread across monthly sheets and is not fully consistent in naming or structure. This project brings the data into one consolidated view, applies the required revenue correction, analyses profitability, and presents the results through an executive-style dashboard.

The goal was not just to make charts. The main focus was to answer a few useful business questions:

- How much revenue and operating profit did the business generate in H1 2024?
- Which product lines are creating or reducing margin?
- Which European markets are performing best?
- How did margins move month by month?
- What should management investigate or act on next?

## Key results

| KPI | H1 2024 result |
|---|---:|
| Corrected Revenue | **€4.57M** |
| Gross Margin | **42.69%** |
| Operating Profit | **€1.23M** |
| Operating Margin | **26.91%** |
| Countries | **4** |
| Product Lines | **5** |
| Customer Segments | **2** |
| Period Covered | **Jan–Jun 2024** |

### A few takeaways

**Automation Software** stands out as the strongest product line, with a **64.35% gross margin**. It is comfortably ahead of the other categories and is the clearest area for growth-focused selling.

**Connectors & Cables** is the weakest product category at **28.91% gross margin**. Its lower margin makes it the first place to look at pricing, supplier costs, discounting, and product mix.

At the regional level, **France leads at 43.89% gross margin**, while **Germany is lowest at 40.53%**. The analysis points to a mix issue and weaker economics within parts of the German portfolio rather than a broad cost problem across the whole business.

Margins were under the most pressure in **February (40.95%) and March (40.03%)**, before improving through the later months. **June reached 44.18%**, the strongest monthly gross margin in the H1 period.

## Data and analysis workflow

The workbook follows a simple reporting flow:

`Monthly source sheets → Combined data → Analysis → Dashboard → Recommendations`

### Source data

The workbook contains six monthly sheets:

- `Jan_2024`
- `Feb_2024`
- `Mar_2024`
- `Apr_2024`
- `May_2024`
- `Jun_2024`

The source tables contain fields covering country, product line, customer segment, revenue, cost of goods sold, operating expenses, units sold, and month.

### Consolidation

`Combined_Data` is the central working table. It standardizes the monthly data into a common structure and includes the corrected revenue field used for the financial analysis.

### Analysis

The `Analysis` sheet summarizes the business from several angles:

- monthly revenue and profitability
- product-level gross margin
- regional gross margin
- overall H1 performance

### Dashboard

The `dashboard` sheet turns the analysis into an executive-facing view with charts for:

- Gross Margin % by Product Line
- Gross Margin % by Region
- H1 monthly profitability trend

### Recommendations

The `Insights Recommendations` sheet translates the numbers into practical next steps, including data governance, sales incentives, hardware profitability, and investigation of the Q1 margin decline.

## Important data-quality point

One of the main analytical findings is a **localized German VAT reporting issue** in the source data. After correcting the affected revenue basis and consolidating the datasets, Germany's position changed materially and became the lowest-margin region in the comparison.

This is a useful reminder that a dashboard is only as reliable as the financial definitions behind it. Before using a similar report for live management decisions, the source data and tax treatment should be formally validated.

## Tools used

- **Microsoft Excel** — data preparation, analysis, dashboarding and reporting
- **Pivot-style summaries / aggregated analysis** — to compare product, regional and monthly performance
- **Charts and executive reporting** — to make the results easier to review and discuss

## Workbook structure

```text
DeltaTech-Financial-Dashboard-GitHub/
├── Portfolio_Khairnar_DeltaTech_Dashboard.xlsx
├── README.md
├── DATA_DICTIONARY.md
├── PROJECT_NOTES.md
├── .gitignore
└── images/
    └── dashboard-preview.png
```

## How to use the workbook

1. Download `Portfolio_Khairnar_DeltaTech_Dashboard.xlsx`.
2. Open it in Microsoft Excel or a compatible spreadsheet application.
3. Start with the `dashboard` sheet for the high-level view.
4. Use `Analysis` to see the supporting numbers.
5. Review `Combined_Data` when you want to trace the consolidated dataset.
6. Use the monthly sheets to inspect the original inputs.
7. Read `Insights Recommendations` for the business interpretation and proposed actions.

## What I would improve in a production version

For a real reporting environment, I would take this one step further by moving the data-cleaning process into a repeatable ETL workflow, adding automated data-quality checks, locking the financial definitions used for revenue and tax treatment, and connecting the final model to a refreshable reporting layer.

That would reduce manual handling and make the dashboard easier to maintain when new months are added.

## Project purpose

This project demonstrates practical skills in:

- financial data cleaning and consolidation
- business and profitability analysis
- KPI reporting
- management dashboard design
- data-quality investigation
- turning analysis into business recommendations

## Repository note

The Excel workbook is the main project file. The PNG image is included only to give visitors a quick preview without opening Excel.

---

### Suggested GitHub repository description

> Excel financial analytics dashboard for DeltaTech B.V. covering H1 2024 revenue, profitability, product margins, regional performance, data-quality corrections, and business recommendations.

### Suggested GitHub topics

`excel` `financial-analysis` `business-analytics` `dashboard` `data-analysis` `kpi` `profitability-analysis` `data-cleaning` `portfolio-project` `management-reporting`
