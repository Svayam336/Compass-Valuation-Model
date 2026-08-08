  # Comprehensive Valuation Model: Compass Group PLC (CPG)

An integrated 3-statement financial model, discounted cash flow (DCF) valuation, trading comps benchmarking, leveraged buyout (LBO) analysis, and automated Python data pipeline for Compass Group PLC.

---

## Executive Summary & Investment Thesis

**Recommendation:** OVERVALUED at $31.71  
**Implied DCF Fair Value:** $26.51 – $28.29 (~10.8% to 16.4% Downside)

Compass Group is a premium operational performer trading at an ultra-premium price. While the company demonstrates clear operational superiority within the contract catering space, the market has fully priced in flawless execution. The current entry point offers a severely limited margin of safety for both public investors and private equity buyers.

### Key Drivers of the Thesis

* **DCF Analysis:** Even when applying healthy growth assumptions (6.6%–8.0% 5-year revenue growth), the baseline DCF indicates the stock is trading above intrinsic value. Assuming an 8.0% WACC and an 11.0x terminal EBITDA multiple, the implied share price sits at **$28.29** (10.8% downside). Using a 3.0% perpetuity growth rate suggests an even steeper **16.4% downside to $26.51**.
* **Relative Valuation to Comps:** Compass has superior operating metrics, projecting a FY26 EBITDA margin of 9.1% compared to the peer median of just 6.8%. However, this operational edge does not justify the significant trading premium. Compass currently trades at 13.9x FY26 EV/EBITDA—a massive ~54% premium over the peer median of 9.0x. The market has already rewarded the company for its efficiency, leaving no room for multiple expansion.
* **LBO Returns Analysis:** A sponsor take-private is largely unfeasible at current trading levels. A standard 25% share price premium forces a steep 17.2x entry valuation, while the current high-rate environment constrains entry leverage and debt paydown capacity. Under these conditions, our 14.0x base exit yields an insufficient ~5% IRR. To achieve a baseline 20% return without relying on unrealistic multiple expansion, a buyer would have to drastically reduce their entry valuation, solving to a maximum justifiable share price significantly below current trading levels.

---

## Model Drivers & Key Assumptions

| Operating Assumptions | DCF Assumptions | LBO Assumptions |
| :--- | :--- | :--- |
| **5-Yr Revenue Growth:** 6.6% – 8.0% | **Calculated WACC:** 8.0% | **Entry Valuation:** 17.2x TEV / EBITDA |
| **Direct Operating Costs:** ~90.6% Rev | **FCF Terminal Growth Rate:** 3.0% | **Offer Premium:** 25.0% |
| **Effective Tax Rate:** 27.7% | **Terminal EBITDA Multiple:** 11.0x | **Entry Leverage:** 6.3x Debt / EBITDA |
| **CapEx Requirement:** ~3.0% of Rev | **Unlevered Beta:** 0.69 | **Weighted Debt Cost:** 7.7% |
| **NWC Intensity:** ~35.6% of Rev | **Risk-Free Rate:** 4.9% | **Base Exit Multiple (FY30):** 14.0x |

---

## Valuation Summary

| Valuation Methodology | Implied Share Price | Premium / (Discount) to Current ($31.71) |
| :--- | :--- | :--- |
| **DCF: Terminal Multiple (11.0x)** | $28.29 | (10.8%) |
| **DCF: Perpetuity Growth (3.0%)** | $26.51 | (16.4%) |
| **Comps: FY26 EV/EBITDA (25th–75th Pct)** | $8.97 – $20.27 | (36.1%) to (71.7%) |
| **LBO Target Price (for 20% Sponsor IRR)** | < $20.00 | > (37.0%) |

---

## Automated Data Pipeline

This repository includes an automated Python data pipeline built in Jupyter Notebook (`data_pipeline.ipynb`). Using the `yfinance` API, the script programmatically fetches live financial statement data, market statistics, and peer valuation metrics, exporting structured datasets directly into CSV format for integration into the Excel financial model.

---

## Repository File Structure

* `Compass Project.xlsx`: Master financial model containing:
  * `Dashboard`: Executive summary, assumption panels, football field valuation summary, and investment thesis.
  * `3_Statement_Model`: Integrated 3-statement historical and forecast model (FY23–FY30).
  * `DCF`: Unlevered Free Cash Flow projections, WACC build, and sensitivity tables.
  * `Comps`: Peer group trading stats, multiples, and summary statistical distributions.
  * `LBO`: Transaction sources & uses, debt schedules, returns, and IRR sensitivity matrices.
* `compass_data_pipeline.ipynb`: Jupyter Notebook automated data extraction pipeline using `yfinance`.
* `data/`: Directory containing raw CSV data exports (`compass_balance_sheet_3yr.csv`, `compass_cash_flow_sheet_3yr.csv`, `compass_income_statement.csv`).
* `README.md`: Executive dashboard summary and formal investment thesis.
