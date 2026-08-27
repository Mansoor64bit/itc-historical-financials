# 📊 ITC Limited — Historical Financial Statement Analysis (FY2017–FY2026)

> A decade-long, ground-up financial model of ITC Limited built entirely in Excel — standardising ten years of consolidated financials into one consistent framework, then layering common-size analysis, ratio analysis, and forward forecasting on top.

---

## 🧭 Project Overview

Reading a company's financials one annual report at a time hides the story. Trends only become visible when a decade of numbers sits side by side in a single, consistently-formatted model.

This project consolidates **ITC Limited's consolidated financial statements from FY2017 through FY2026** into a single Excel workbook, then builds out common-size statements, a 16+ ratio analysis suite, and a 5-year forward projection model for Sales, EBITDA, and EPS. The result reads less like a spreadsheet and more like the backbone of an equity research note.

**Headline numbers from the model:**
- Revenue grew from ₹42,768 Cr (FY17) to ₹78,868 Cr (FY26) — a **7.04% CAGR**
- PAT grew from ₹8,719 Cr to ₹18,495 Cr — an **8.72% CAGR**, outpacing revenue growth
- ROCE stands at **34.17%** (FY26), averaging **30.60%** over the decade
- The company carries almost no debt: **D/E of 0.033x** against **₹41,137 Cr** in cash + investments

---

## 🎯 Business Problems Solved

| Problem | What This Model Does |
|---|---|
| Ten years of annual report data is fragmented and inconsistent | Consolidates FY17–FY26 financials into one continuous, comparable format |
| Raw statements don't reveal structural trends | Common-size statements isolate cost, margin, and tax-rate trends as % of sales/assets |
| Financial health needs a scorecard, not just three statements | 16+ pre-built ratios spanning profitability, leverage, liquidity, and efficiency |
| Historical data alone doesn't inform forward decisions | A weighted forecasting model projects Sales, EBITDA, and EPS 5 years out |

---

## 📁 Repository Structure

```
itc-historical-financial-analysis/
│
├── 📂 model/
│   └── ITC_Historical_FS_Model.xlsx        
│
├── 📂 documentation/
│   └── ITC_Metrics_Impact_Report.docx     
│
├── 📂 screenshots/
│   ├── 01_revenue_pat_trend.png
│   ├── 02_margin_trend.png
│   ├── 03_ratio_analysis_summary.png
│   ├── 04_common_size_statement.png
│   └── 05_forecasting_output.png
│
├── README.md
└── LICENSE
```

---

## 🔬 Model Architecture

The workbook is built across five linked sheets:

### 1. `Historical FS`
The core historical Income Statement, Balance Sheet, and Cash Flow Statement — FY2017 through FY2026, plus a trailing-twelve-month (LTM) column. Includes Sales, COGS, Gross Profit, EBITDA, EBIT, PBT, Tax, Net Profit, EPS, DPS, and Dividend Payout Ratio, alongside Balance Sheet items (Equity, Reserves, Borrowings, Assets) and the three Cash Flow lines.

### 2. `Common Size Statement`
Every Income Statement and Balance Sheet line expressed as a % of Sales / Total Assets respectively — the fastest way to see structural shifts (e.g., raw material cost as % of sales, or the changing mix of the balance sheet) that raw numbers hide.

### 3. `Ratio Analysis`
16+ ratios computed year-by-year with trend, mean, and median columns: Sales/EBITDA/EBIT/Net Profit/Dividend growth, margin ratios, ROCE, ROE, Self-Sustained Growth Rate, Interest Coverage, Turnover ratios (Debtor/Creditor/Inventory/Fixed Asset/Capital), Debtor/Payable/Inventory Days, Cash Conversion Cycle, and CFO-based ratios (CFO/Sales, CFO/Total Assets, CFO/Total Debt).

### 4. `Forecasting`
A weighted historical-growth projection model extending Sales, EBITDA, and EPS five years beyond the last actual reporting period.

### 5. `Data Sheet`
The locked master data sheet feeding all other tabs — includes market data (share price, market cap, shares outstanding) alongside quarterly figures and the full annual data set.

---

## 💡 Core Insights Discovered

**1. Profit Is Compounding Faster Than Revenue**
PAT CAGR (8.72%) has outpaced Revenue CAGR (7.04%) over FY17–FY26 — a sign of genuine margin expansion, not just scale.

**2. A Structurally Falling Tax Rate Has Been a Quiet Tailwind**
The effective tax rate declined from ~38.9% in FY2017 to ~27.5% in FY2026 — an ~11 percentage-point drop that has materially boosted PAT growth independent of operating performance.

**3. A Genuinely Debt-Free Balance Sheet**
Debt-to-Equity sits at just 0.033x in FY2026, against ₹41,137 Cr in cash and investments combined — the company is, for practical purposes, a net-cash business.

**4. Capital Return Has Outpaced Earnings Growth**
DPS compounded at 13.20% CAGR — faster than both revenue and profit growth — with the payout ratio averaging 93.28% over the decade and hitting 98.23% in FY2026.

**5. Working Capital Has Loosened**
The Cash Conversion Cycle nearly doubled from 43.1 days (FY23) to 90.1 days (FY26), driven largely by inventory days rising from 112 to 159 — a trend worth watching going forward.

**6. Returns on Capital Have Improved, Not Just Held Steady**
Both ROE (17.6% → 25.5%) and ROCE (29.1% → 34.2%) trended upward over the decade despite a growing capital base — incremental capital has been deployed productively, not just accumulated.

---

## 🛠️ Tech Stack

| Tool | Role |
|---|---|
| **Microsoft Excel** | Full financial modelling — Historical FS, Common-Size Statements, Ratio Analysis, Forecasting |
| **ITC Financial Filings** | Primary data source (FY2017–FY2026, consolidated basis) |

---

## 📸 Screenshots

> *(Replace each placeholder below with an actual screenshot from your Excel model)*

### Revenue & PAT Trend — FY2017 to FY2026
![Revenue and PAT Trend](screenshots/01_revenue_pat_trend.png)

### Margin Trend (Gross / EBITDA / Net Profit)
![Margin Trend](screenshots/02_margin_trend.png)

### Ratio Analysis Summary
![Ratio Analysis](screenshots/03_ratio_analysis_summary.png)

### Common Size Statement
![Common Size Statement](screenshots/04_common_size_statement.png)

### Forecasting Output
![Forecasting Output](screenshots/05_forecasting_output.png)

---

## 🚀 How to Use This Model

1. **Clone the repository**
   ```bash
   git clone https://github.com/[your-username]/itc-historical-financial-analysis.git
   ```

2. **Open the main model**
   Navigate to `model/ITC_Historical_FS_Model.xlsx` and open in Microsoft Excel.

3. **Start with the `Historical FS` tab**, then move through `Common Size Statement` → `Ratio Analysis` → `Forecasting`. The `Data Sheet` tab is the locked source layer — do not edit it directly.

---

## 📌 Data Sources & Disclaimer

- Data sourced from ITC Limited's publicly available financial filings (consolidated basis)
- This model is built for **educational and analytical purposes only** — not investment advice

---

## 👤 Author

**[Your Name]**
[LinkedIn Profile] · [Email] · [Portfolio]

---

## ⭐ If this project was useful

Give it a star ⭐ — it helps others find it and lets me know the work was worth sharing.
