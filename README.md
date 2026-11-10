# Date-Aware KPIs & Revenue Analysis (Power BI)

A Power BI report focused on time intelligence: year-to-date revenue, year-over-year comparison, revenue share by region, and actual-vs-target variance.

## What the Dashboard Shows
- **Monthly Revenue** by year-month
- **Revenue YTD** running total across the year
- **Total Revenue vs Previous Year Revenue** comparison
- **Revenue Growth %** by month
- **Revenue Share of All Regions** per region
- **Revenue Target vs Actual** with variance by region and month
- **Year slicer** (2025 / 2026)

## DAX Measures
- `Total Revenue`
- `Revenue YTD`
- `previous Year Revenue`
- `Revenue Growth %`
- `Revenue All Regions`
- `Revenue Share %`
- `Revenue Variance`
- `variance%`

## Data Model
Star schema built on `Fact_Orders` (Order_ID, Customer_ID, Order_Date, Qty, Unit_Price, Discount_Pct, Revenue, Status) with `Dim_Customer`, `Dim_Course`, `Dim_Region`, `Dim_Date` and a `Targets` table.

## Highlights
- Total revenue of ₹29,10,369 across all regions (2025)
- Region split: East ₹7,55,940 · South ₹7,55,940 · West ₹7,18,143 · North ₹6,80,346
- Uses a proper date table so YTD and previous-year measures work correctly

## Tools
Power BI Desktop · DAX (time intelligence) · Power Query

## How to Use
Download the `.pbix` file and open it in Power BI Desktop.

## Repository Contents
```
├── README.md
├── screenshots/dashboard.png    # dashboard preview
└── model-files/                 # internal Power BI model parts
    ├── DataModel
    ├── DiagramLayout
    ├── Metadata
    ├── SecurityBindings
    ├── Settings
    ├── Version
    └── [Content_Types].xml
```
