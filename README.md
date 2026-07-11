# MD ProMax — Executive Dashboard (Power BI)

A Power BI dashboard built for Managing Director–level review of a project-driven engineering business (conveyor / material handling systems for power, cement, coal, and railway customers). It consolidates order book, revenue, project execution, collections, P&L, and manpower into a single report for monthly leadership reviews.

## 📁 Contents

| File | Description |
|---|---|
| `md_promax.pbix` | Power BI report file (data model + report pages) |
| `MD_Dashboard_Data.xlsx` | Source data workbook feeding the report |

## 📊 Report Pages

The `.pbix` contains 6 report pages:

1. **Revenue Summary** — Monthly booked orders, invoiced amount, collections, outstanding, target vs. achievement %
2. **Project Status Tracker** — Live status of ongoing projects (contract value, % complete, invoiced-to-date, balance to invoice, delays, PM ownership)
3. **Order Book** — Open sales orders by customer/segment, balance to execute, expected completion, priority
4. **Collections** — Invoice-wise collection tracking, days-to-collect, payment mode, outstanding
5. **PnL Summary** — Quarterly P&L (Revenue → Material Cost → Gross Profit → EBITDA → EBIT → PBT) with FY26 vs FY25 and YoY growth
6. **HR** — Departmental headcount, on-site/office/contractor split, open positions, attrition, average experience

## 🗂️ Data Model

Sourced from `MD_Dashboard_Data.xlsx`, which contains 6 tables:

- `Revenue_Summary` — Monthly revenue & collections vs. target
- `Project_Status` — Project-level execution tracker
- `PnL_Summary` — Quarterly P&L statement
- `OrderBook` — Open order book by sales order
- `Collections` — Invoice/payment-level collection log
- `Manpower_Summary` — Department-wise headcount and attrition

## 🚀 Getting Started

1. Clone/download this repository.
2. Open `md_promax.pbix` in **Power BI Desktop** (2024+ recommended).
3. If prompted, point the data source to your local copy of `MD_Dashboard_Data.xlsx`, or update the source path via **Transform Data → Data Source Settings**.
4. Refresh the data model.

## 🔄 Updating the Data

To refresh the dashboard with new figures:
1. Update the relevant sheet(s) in `MD_Dashboard_Data.xlsx` (keep column headers unchanged so relationships/measures don't break).
2. Open `md_promax.pbix` in Power BI Desktop and click **Refresh**.
3. Publish to Power BI Service if sharing online.

## 🛠️ Requirements

- Power BI Desktop (May 2026 release or later)
- Microsoft Excel (to edit the source workbook)

## 📌 Notes

- All financial figures are in INR.
- This is a sample/demo data set — customer, project, and financial values are illustrative, not production data.

## 📄 License

Add a license of your choice (e.g., MIT) if this repository is public.
