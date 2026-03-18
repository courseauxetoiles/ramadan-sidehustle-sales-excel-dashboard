# Ramadan 2026 Beverage Business — Financial Tracking & KPI Dashboard (Excel)

> A real-world Excel system built to track, analyze, and optimize a live beverage business operated during Ramadan 1447H (February–March 2026).

---

## Overview

This project documents the complete financial tracking system I built for my own side hustle — a beverage stall I operated during Ramadan 2026 in Surabaya, Indonesia. Over three active selling sessions, I sold handcrafted drinks including temulawak, grass jelly, and banana-based beverages at a fixed price of Rp 4,000 per cup, fulfilling hundreds of orders per session.

Rather than tracking everything manually on paper or in a basic notes app, I designed a structured Excel workbook from scratch to manage the full financial lifecycle of the business — from raw ingredient costs to net profit per session. The system evolved into a professional-grade analytical tool complete with a KPI dashboard, automated calculations, and actionable business insights.

This is not a sample dataset or practice exercise. Every number in this workbook reflects a real transaction.

---

## Business Problem

Running a small food and beverage operation during Ramadan comes with several operational pressures:

- **Short selling windows** — each session lasts only a few hours, leaving no time for manual calculations mid-operation
- **Variable costs** — ingredient prices fluctuate across sessions (e.g., sugar prices, ice block sourcing), making it hard to track true margins without a system
- **Multiple cost categories** — raw materials, operational supplies, and labor all need to be tracked separately to understand where money is actually going
- **No historical baseline** — without structured records, it is impossible to compare sessions, spot cost patterns, or make smarter decisions for the next outing
- **Profit sharing** — with a business partner involved, accurate and transparent financial records are essential

A lightweight, auditable, formula-driven Excel system was the right solution: fast to build, easy to update in the field, and powerful enough to surface real insights.

---

## Solution

I built a six-sheet Excel workbook that takes raw transaction data as input and automatically produces a full financial summary and visual KPI dashboard as output. The system is structured around a clear data flow:

```
Raw Data  →  Summary  →  Product Analysis  →  Dashboard
```

All calculations are formula-driven — no values are manually hardcoded into summary cells. This means the entire workbook updates automatically whenever a new session's data is entered into the Raw Data sheet. The dashboard gives an at-a-glance view of the business health across all sessions, while the underlying sheets support deeper cost and product-level analysis.

---

## Key Features

### Transaction Ledger (Raw Data)
- Structured double-entry-style log: every cash inflow and outflow is recorded with date, category, description, quantity, and unit price
- Dynamic running balance column updates automatically as rows are added
- Income rows are visually distinguished from expense rows for fast readability
- AutoFilter enabled for date, type, and category slicing

### Automated Financial Calculations
- Session-level revenue, cost, and profit calculated using `SUMIFS` with date and type filters — no manual aggregation needed
- Profit margin computed dynamically per session and in aggregate
- Cumulative profit tracked across sessions to show business trajectory
- Cost breakdown by category (Raw Materials / Operational / Labor) expressed both in absolute IDR and as a percentage of revenue

### Product & Ingredient Analysis
- Full item-level breakdown of every ingredient and supply purchased across all sessions
- Tracks total quantity consumed, last known unit price, total spend, and frequency of purchase
- Each item's share of total cost calculated automatically
- Helps identify high-impact cost drivers at a glance

### KPI Dashboard
- Six top-level KPI cards: Total Revenue, Total Cost, Net Profit, Profit Margin, Total Units Sold, and Average Order Value
- Supporting metrics: highest-profit session, lowest-margin session, average units per session
- Three embedded charts: clustered bar chart (revenue vs. cost vs. profit by session), pie chart (cost breakdown by category), and line chart (profit margin trend across sessions)
- Key Insights section with six data-driven business recommendations derived directly from the numbers
- Fully formula-driven — no values are hardcoded into the dashboard

### Professional Formatting
- Corporate-standard design: neutral navy/blue/white color palette, no decorative elements
- Industry-standard color coding: blue text for hardcoded inputs, black for formulas, green for cross-sheet references
- Accounting number format throughout (IDR, thousands separator, parentheses for negatives)
- Frozen header rows, AutoFilter, and tab color-coding for fast navigation

---

## Tools & Skills

| Area | Details |
|---|---|
| **Microsoft Excel** | Workbook architecture, multi-sheet design, named ranges |
| **Formulas** | `SUMIF`, `SUMIFS`, `IF`, `AVERAGE`, `MAX`, `MIN`, `COUNTA`, `SUM`, `IFERROR` |
| **Data Architecture** | Input → Processing → Output sheet structure; separation of raw data from calculated outputs |
| **Financial Analysis** | Margin analysis, cost breakdown, cumulative profit tracking, break-even estimation |
| **Dashboard Design** | KPI card layout, chart embedding, insight narrative, corporate visual standards |
| **Business Thinking** | Translating real operational questions into trackable metrics and actionable outputs |

---

## Data Structure

| Sheet | Purpose |
|---|---|
| **Dashboard** | Executive summary view. Opens first. All KPIs, charts, and business insights in one place. |
| **Raw Data** | Single source of truth. Every transaction from every session is logged here. |
| **Summary** | Aggregated financials. Daily session performance and cost breakdown by category. |
| **Product Analysis** | Item-level cost breakdown. Every ingredient and supply with quantity, cost, and cost share. |
| **_ChartData** | Hidden helper sheet. Structured data ranges that feed all dashboard charts. |
| **Assumptions** | All hardcoded inputs documented in one place. Selling price, targets, operational notes. |

---

## KPIs & Insights

### Metrics Tracked

| Metric | Value (3 Sessions) |
|---|---|
| Total Revenue | Rp 3,052,000 |
| Total Cost | Rp 1,194,900 |
| Net Profit | Rp 1,857,100 |
| Profit Margin | 60.85% |
| Total Units Sold | 763 cups |
| Average Order Value | Rp 4,000 / cup |
| Best Margin Session | 3 March 2026 (72.3%) |
| Avg Units per Session | ~254 cups |

### Key Business Insights Surfaced by the System

1. **Session 2 (3 March) was the most efficient** — same revenue as Session 3 but lower cost, driven by a simpler ingredient list. This suggests that streamlining the menu improves margins without sacrificing volume.

2. **Banana costs were a significant risk in Session 3** — accounting for 33.7% of that session's total expenditure. Bulk purchasing or price negotiation with the supplier would materially improve profitability.

3. **Fixed pricing at Rp 4,000/cup is stable but limiting** — the system reveals headroom to introduce a premium product variant at a higher price point without disrupting the core offering.

4. **Break-even is achieved very early** — approximately Rp 160,000 in revenue covers fixed labor costs, which is reached within the first 40 cups sold. The business has a favorable risk profile.

5. **Raw materials dominate the cost structure at 63%** — the single highest-leverage improvement is supplier negotiation and bulk procurement planning before each session.

6. **A target of 300 cups per session is realistic** — the gap from the current average (254) to the target is 18%. Achieving it would improve fixed-cost absorption and push overall margin above 65%.

---

## How to Use

**To log a new session:**
1. Open the **Raw Data** sheet
2. Add each transaction as a new row: date, type (Income / Expense), category, description, quantity, and unit price
3. Copy the Debit, Credit, and Balance formulas from the row above — they will auto-calculate
4. All summary figures, charts, and KPIs on the Dashboard will update automatically

**To review performance:**
- Go to the **Dashboard** sheet for the full picture
- Go to **Summary** for a session-by-session breakdown
- Go to **Product Analysis** to review ingredient costs

**To adjust assumptions:**
- Open the **Assumptions** sheet
- Update any blue-text values (e.g., selling price, target volume)
- All dependent calculations will recalculate automatically

> No manual editing of formula cells is required. All black-text cells are calculated automatically.

---

## Key Learnings

Building this system for a live business — under real time pressure, with real money on the line — produced a different quality of learning than any classroom or tutorial project.

- **Data architecture matters immediately** — a poorly structured Raw Data sheet would have made every downstream formula fragile. Designing it right from the start saved hours of debugging mid-operation.
- **Business questions drive better analysis** — instead of building generic charts, every metric in this workbook answers a specific question I actually needed answered (e.g., "Which session had the best margin, and why?").
- **Formulas are only as good as the assumptions behind them** — separating hardcoded inputs into a dedicated Assumptions sheet made the model transparent, auditable, and trustworthy.
- **Small businesses generate rich data** — even three sessions of a street-level beverage stall produce enough structured data to drive meaningful strategic decisions.
- **Process documentation has compounding value** — by the third session, setup time dropped significantly because the system was already built and waiting.

---

## Future Improvements

| Improvement | Description |
|---|---|
| **Session Forecasting** | Add a projection tab that estimates profit for the next session based on historical averages and a configurable volume target |
| **Ingredient Price Tracker** | Track unit price changes across sessions to model supplier price trends and flag cost increases |
| **Google Sheets Migration** | Port the workbook to Google Sheets for real-time mobile access during operations |
| **Profit Sharing Calculator** | Automate the 50/50 partner split calculation with a dedicated output per session |
| **Inventory Pre-Planning Sheet** | Add a pre-session sheet that calculates required ingredient quantities based on a target cup volume |
| **Power BI Dashboard** | Migrate the dashboard to Power BI for richer interactivity and easier sharing with business partners |

---

## Author

**[Raihan Ahmad Abiyyu]**
Data Analyst | Excel & Business Intelligence | Surabaya, Indonesia

- GitHub: [github.com/yourusername](https://github.com/courseauxetoiles)
- LinkedIn: [linkedin.com/in/yourprofile](https://linkedin.com/in/raihanabiyyu)

---

> _This project is based on a real business operation conducted during Ramadan 1447H (February–March 2026). All financial figures are actual recorded values._
