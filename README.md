# ITC Ltd. — Historical Financial Statements & Ratio Analysis

A 10-year historical financial model for **ITC Ltd.** (FY2017–FY2026, plus LTM and the last 10 quarters), with a common-size statement, a full ratio analysis dashboard, and a simple trendline forecast out to FY2031.

![Historical Financial Statements](screenshots/01_historical_financial_statements.png)

## What this is

This model takes ITC's reported Income Statement, Balance Sheet, and Cash Flow Statement for FY2017 through FY2026 (year ending 31 March), restates them into a clean, formula-linked historical financial statement, then layers on:

- **Common-size statements** (every line as a % of Sales / Total Assets, to compare cost structure across years)
- **Ratio analysis** (growth, margins, returns, turnover, working-capital days, cash-flow coverage — with 10-year mean and median for each)
- **A trendline forecast** (Sales, EBITDA, and EPS projected out to FY2031 using linear regression off the 10-year history)

All numbers are in ₹ Crore unless stated otherwise (per-share figures in ₹).

## Files

| File | Description |
|---|---|
| `ITC_Historical_Financial_Statements.xlsx` | The model — 5 tabs, fully formula-linked |
| `Report.docx` | Written summary of the numbers, trends, and what stands out |
| `screenshots/` | Visual snapshots of each tab |

## Tabs in the model

1. **Historical FS** — Income Statement, Balance Sheet, and Cash Flow Statement, FY2017–FY2026 + LTM. Includes a balance-sheet check row (Total Assets = Total Liabilities, confirmed `TRUE` for every year).
2. **Common Size Statement** — Income Statement and Balance Sheet, every line expressed as a % of Sales / Total Assets respectively.
3. **Ratio Analysis** — Growth rates (Sales, EBITDA, EBIT, Net Profit, Dividend), margins, capital efficiency (ROCE, ROE, Self-Sustained Growth Rate), turnover ratios, working-capital days, and cash-flow coverage ratios — each with a 10-year mean and median.
4. **Forecasting** — Sales, EBITDA, and EPS projected for FY2027–FY2031 using Excel's `FORECAST()` (linear trendline regression) off the FY2017–FY2026 actuals.
5. **Data Sheet** — The raw source data feeding every other tab (annual P&L/BS/CF, quarterly P&L, and share price by quarter). Marked "please do not make any changes" in the original file — treat as the single source of truth and update figures here only.

Every ratio, margin, and forecast is a **live formula**. Update the Data Sheet with a new year's results and the other four tabs recalculate automatically.

## Key numbers (FY2017 → FY2026)

| Metric | FY2017 | FY2026 | 10-yr Mean | 10-yr Median |
|---|---|---|---|---|
| Sales (₹ Cr) | 42,768 | 78,868 | — | — |
| Sales Growth | — | 4.71% | 7.35% | 4.71% |
| EBITDA Margin | 36.17% | 34.62% | 36.26% | 36.21% |
| Net Profit Margin | 20.39% | 23.45% | 23.15% | 22.66% |
| EPS (₹) | 7.18 | 14.76 | — | — |
| Return on Equity | 18.78% | 25.51% | 21.31% | 20.98% |
| Return on Capital Employed | 30.82% | 34.40% | 30.60% | 30.47% |
| Interest Coverage | 292x | 301x | 321x | 296x |

Revenue grew at roughly a **7% CAGR** and EPS at roughly an **8% CAGR** over the decade, on a business that runs with almost no debt (interest coverage consistently above 200x). One year needs a footnote: **FY2025's common-size net margin jumps to ~46%** (versus a "normal" ~23–25% range) because that year's Other Income includes a large one-off gain — the Historical FS tab's Net Profit figure for FY2025 (₹17,250 Cr) already strips this out, but the Data Sheet / Common Size tabs' raw P&L figure (₹34,747 Cr) does not. See the caveat in `Report.docx` for the full explanation.

## How to use it

1. Open `ITC_Historical_Financial_Statements.xlsx` in Excel or Google Sheets.
2. Update the **Data Sheet** tab as new quarterly/annual results are published — that's the only tab meant to be edited directly.
3. The Historical FS, Common Size, Ratio Analysis, and Forecasting tabs all recalculate automatically.
4. To extend the forecast horizon, add more rows to the Forecasting tab following the same `FORECAST()` pattern.

## Disclaimer

This is a historical-data and ratio-analysis workbook built from reported financials, not investment advice. The forecast tab is a simple linear trendline projection (not a business-driven bottom-up forecast) and should be treated as illustrative only — it doesn't account for one-off items, changing tax rates, or forward business guidance.
