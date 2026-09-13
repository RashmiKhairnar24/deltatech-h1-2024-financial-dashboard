# Data Dictionary

This file explains the main fields used in the consolidated workbook.

| Field | Meaning | Notes |
|---|---|---|
| Country | Sales market / reporting country | Netherlands, Germany, Belgium, France |
| ProductLine | Product category | Five categories are covered |
| CustomerSegment | Customer type | Enterprise or SMB |
| Revenue_EUR | Source revenue field | Present in the monthly source sheets |
| Revenue_EUR_Corrected | Revenue used for the consolidated analysis | Corrected financial basis used in the analysis |
| COGS_EUR | Cost of goods sold | Used to calculate gross profit and gross margin |
| OperatingExpenses_EUR | Operating expenses | Used to calculate operating profit |
| OperatingExpenses_Eur2 | Consolidated operating expense field | Used where present in the combined dataset |
| UnitsSold | Units sold | Used as an operational sales measure |
| Month | Reporting month | Jan–Jun 2024 |

## Main calculations

**Gross Profit**

`Revenue_EUR_Corrected - COGS_EUR`

**Gross Margin %**

`Gross Profit / Revenue_EUR_Corrected`

**Operating Profit**

`Gross Profit - Operating Expenses`

**Operating Margin %**

`Operating Profit / Revenue_EUR_Corrected`

## Data-quality observations

The monthly source sheets are not perfectly standardized. Examples include differences in capitalization and naming such as `Industrial sensors`, `INDUSTRIAL SENSORS`, and `Industrial Sensors`.

There are also some missing operating-expense values and a localized German VAT-related revenue issue identified during analysis. These points should be checked carefully before the workbook is used for audited or operational reporting.
