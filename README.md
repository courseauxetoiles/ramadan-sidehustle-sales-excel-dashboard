# 🥤 Ramadan Beverage Order Tracker
### Real Business Financial Dashboard — Built & Operated During Ramadan 1447H

![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

---

## 📌 Project Overview

This is a **real business I ran during Ramadan 1447H** — selling beverages per order across multiple sessions throughout the month. To manage finances properly, I built this Excel workbook from scratch to track every transaction, monitor daily profitability, and make smarter purchasing decisions in real time.

What started as a simple order log evolved into a full financial reporting system: a structured transaction ledger, automated daily summaries, ingredient-level cost breakdowns, and a management dashboard — all built while the business was actively running.

> This isn't a mock project or tutorial exercise. Every number in here is real — real orders, real costs, real profit.

---

## 🧩 Background & Problem Statement

Running a small beverage business during Ramadan is fast-paced. Orders come in, ingredients need to be bought before each session, and costs shift week to week. Early on I tracked everything manually — and quickly ran into real problems:

- 📋 **No clear record** of what was spent per session on ingredients
- ❌ **Couldn't calculate actual profit** without sitting down and doing it by hand after every run
- 💸 **Ingredient prices varied** between sessions — sugar alone shifted 3.6% in two weeks
- 📊 **No way to compare sessions** — was the 3 March run actually better than 25 February?
- 🤝 **Profit-sharing with a partner** needed to be transparent and verifiable every session

I built this workbook to solve all of that — and to turn the raw hustle of running a Ramadan side business into something I could actually learn from.

---

## ✨ Key Features

### 📂 Multi-Sheet Architecture
- **5 dedicated sheets** covering every aspect of the business
- Color-coded tabs for instant navigation
- Frozen headers and auto-filters on all data sheets

### 💰 Real Transaction Ledger
- Full **cash ledger** (Debit / Kredit / Running Saldo) per session
- Every purchase logged with item name, quantity, and unit price
- Automatic running balance after every line entry

### 📊 Management Dashboard
- 6 KPI tiles: Revenue, Cost, Profit, Margin %, Cups Sold, Price/Cup
- **3 embedded charts**: Revenue vs Cost vs Profit (bar), Margin trend (line), Cost breakdown (pie)
- **Key Insights box** with 6 actionable takeaways from the data

### 🧮 Cost Intelligence
- Item-level breakdown across **21 unique ingredients & supplies**
- Grouped by: Bahan Baku (Raw Materials), Operasional, Tenaga Kerja (Labor)
- Frequency tracking to spot which items are bought every session
- **% of total cost** per item — surfaces the biggest cost drivers instantly

### 📅 Daily Session Summaries
- Side-by-side comparison of all sessions: revenue, costs, profit, and margin
- **Cash position tracking** with opening balance, net movement, and closing balance
- Cumulative saldo rolling across the entire Ramadan period

### ⚙️ Formula-Driven, Easy to Update
- All totals and KPIs built on **Excel formulas** — no manual recalculation
- Color-coded row logic: Income rows (green), Labor (red), alternating rows for readability
- Documented assumptions sheet — easy to adjust if prices or conditions change

---

## 🛠️ Tools & Technologies

| Tool | Usage |
|------|-------|
| **Microsoft Excel** | Core platform for all data, formulas, and charts |
| **openpyxl (Python)** | Programmatic workbook generation and formatting |
| **Excel Formulas** | SUM, AVERAGE, dynamic running balances |
| **Conditional Formatting** | Visual cues for income vs. expense row types |
| **Excel Charts** | Bar, Line, and Pie charts embedded in Dashboard |
| **Data Validation** | Controlled inputs to reduce data entry errors |

---

## 📁 Data Structure

The workbook is organized into **5 sheets**, each serving a distinct purpose:

### 1. `Raw Data` 🔵
> Every single transaction logged — the ground truth of the business.

| Column | Description |
|--------|-------------|
| Tanggal | Transaction date |
| No | Line item number within the session |
| Jenis | `Masuk` (Cash In) or `Keluar` (Cash Out) |
| Kategori | Bahan Baku / Operasional / Tenaga Kerja / Penjualan |
| Keterangan | Item name or description |
| Jumlah (Unit) | Quantity |
| Harga Satuan | Unit price (IDR) |
| Debit | Cash received |
| Kredit | Cash paid out |
| Saldo | Running cash balance for the session |

### 2. `Summary` 🔵
> Aggregated view of financial performance across all sessions.
- KPI metric tiles (Revenue, Cost, Profit, Margin)
- Per-date comparison table with daily laba and margin
- Cost breakdown by category with percentages
- Key ingredient analysis

### 3. `Dashboard` 🟢
> One-page business overview — designed to answer "how are we doing?" at a glance.
- Visual KPI cards and performance charts
- Margin trend, Revenue vs Cost comparison, Cost category split
- Actionable insights panel

### 4. `Product Analysis` 🟠
> Deep-dive into every cost item across all sessions.
- All 21 SKUs with total quantity, unit cost, total spend, and frequency
- Grouped by category with clear section headers
- `% of Total Cost` to identify what's eating into profit

### 5. `Asumsi & Catatan` 🟣
> The assumptions register — the "brain" behind the numbers.
- Selling price, capacity estimates, and profit-split ratio
- Operational notes for running future sessions
- Color-coding legend for the workbook

---

## 📊 Business Results & Insights

Here's what the data actually showed across **3 sessions** (25 Feb – 9 Mar 2026):

| Metric | Value |
|--------|-------|
| Total Revenue | Rp 3,052,000 |
| Total Cost | Rp 1,194,900 |
| **Net Profit** | **Rp 1,857,100** |
| Average Profit Margin | **60.85%** |
| Total Cups Sold | 763 cups |
| Price Per Cup | Rp 4,000 (fixed) |

### 📈 What the Data Revealed
- **Best session**: 3 March 2026 — 72.3% margin, lowest costs of any session
- **Tightest session**: 9 March 2026 — Pisang (banana) alone made up 33.6% of that day's costs
- **Sugar price creep**: Gula was purchased at Rp 16,500 → Rp 17,000 → Rp 16,300 across sessions — inconsistency worth negotiating
- **Break-even point**: Roughly Rp 160,000 per session (labor only) — always hit comfortably

### 💡 Decisions Made From the Data
1. Renegotiate **bulk sugar pricing** — biggest recurring cost at Rp 331,400 total
2. Limit or substitute **Pisang** in high-demand sessions — too price-sensitive
3. Standardise **galon air sourcing** — currently ad-hoc at slightly different prices each time
4. Consider a **Rp 5,000 cup tier** (premium variant) to widen margin further

---

## 🖼️ Screenshots

> *Add screenshots of your workbook here by placing images in a `/screenshots` folder.*

### Dashboard Overview
![Dashboard Preview](screenshots/dashboard_preview.png)

### Daily Summary Table
![Summary Table](screenshots/summary_table.png)

### Raw Data Ledger
![Raw Data](screenshots/raw_data.png)

### Product Cost Analysis
![Product Analysis](screenshots/product_analysis.png)

---

## 🚀 How to Use

### Requirements
- Microsoft Excel 2016 or later
- Basic Excel navigation skills

### Updating After Each New Session

**Step 1 — Open `Raw Data`**
Scroll to the bottom and start a new section for the new session date.

**Step 2 — Log transactions**
Enter each row: date, type (Masuk/Keluar), category, item, quantity, and price. The saldo column updates automatically.

**Step 3 — Update the `Summary` sheet**
Add a new row to the Daily Summary table. KPI tiles will reflect the updated totals.

**Step 4 — Extend chart data ranges**
Right-click each dashboard chart → *Select Data* → extend ranges to include the new session row.

**Step 5 — Review the Dashboard**
Check the insights panel — did margin drop? Did a cost item spike unexpectedly?

> 💡 The whole update takes under 5 minutes once you're familiar with the layout.

---

## 🧠 Skills Demonstrated

Building this while actually running the business meant every feature existed because I genuinely needed it — not because it looked good on a portfolio.

| Skill | How It Shows Up |
|-------|-----------------|
| **Financial Literacy** | Margin analysis, cost categorization, real cash flow tracking |
| **Data Structuring** | Clean, consistent transaction schema across all sessions |
| **Business Intelligence** | KPI design, trend spotting, executive-level dashboard |
| **Excel Proficiency** | Formulas, conditional formatting, charts, filters, freeze panes |
| **Analytical Thinking** | Turning raw costs into actual purchasing decisions |
| **Python / openpyxl** | Programmatic workbook build with full formatting and chart control |
| **Documentation** | Assumptions register, operator guide, color-coding standards |

---

## 🔮 Future Improvements

Things I'd build into the next version if I run this again:

- [ ] **Auto-rollover saldo** — opening balance pulls from previous session automatically
- [ ] **Pre-session budget planner** — estimate costs before going to the market
- [ ] **Target vs. Actual tracker** — set a revenue goal per session, track whether you hit it
- [ ] **Ingredient price history** — track price movement of key items across sessions
- [ ] **Google Sheets version** — update from phone while at the market
- [ ] **WhatsApp order log integration** — parse incoming order messages into the ledger
- [ ] **End-of-Ramadan full P&L report** — one-click summary for the entire month

---

## 📂 Repository Structure

```
ramadan-beverage-tracker/
│
├── 📊 Workbook_Pesanan_Professional.xlsx   # Main workbook (all 5 sheets)
├── 📄 README.md                            # This file
│
└── 📁 screenshots/
    ├── dashboard_preview.png
    ├── summary_table.png
    ├── raw_data.png
    └── product_analysis.png
```

---

## 👤 Author

**[Your Name]**
- 🐙 GitHub: [@your-username](https://github.com/your-username)
- 💼 LinkedIn: [linkedin.com/in/your-profile](https://linkedin.com/in/your-profile)
- 📧 Email: your.email@example.com

---

## 📄 License

This project is licensed under the [MIT License](LICENSE) — feel free to use or adapt it for your own business.

---

<div align="center">

*Built during Ramadan 1447H — from a real order list to a real dashboard* 🌙

⭐ **If this helped you, a star means a lot!** ⭐

</div>
