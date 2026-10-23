# Jaime Pérez Gómez

Quantitative Analysis | Applied Econometrics | Business Operations & Financial Modeling | Personal Projects

---

### Portfolio Overview

This workspace serves as my personal lab for hands-on learning, technical experimentation, and putting quantitative and operational concepts into practice. The projects hosted here explore empirical research and corporate decision modeling using open-source datasets, official public statistics (such as the Bank of Spain and INE), and calibrated simulation frameworks.

Each repository is built to demonstrate methodological rigor, clean data architecture, and practical business criteria: from panel econometric causal inference to in-process OLAP data towers, real estate feasibility, and financial stress-testing.

---

### Core Competencies & Frameworks

| Domain | Methodologies & Frameworks | Tools & Technologies |
| :--- | :--- | :--- |
| **Econometrics & Quantitative Modeling** | Two-Way Fixed Effects (TWFE), Causal Inference, Monte Carlo Simulation, Harberger Deadweight Loss, Tullock Rent-Seeking, Supply Elasticity | Python (`statsmodels`, `linearmodels`, `scipy`), NumPy, Pandas |
| **Corporate Finance & Financial Modeling** | Three-Statement Modeling, Debt Service Coverage (DSCR), Working Capital & CCC Analytics, Countback DSO, Pocket Margin Waterfalls, Stobachoff Whale Curves | Financial Modeling, Scenario Stress-Testing, OpenPyXL |
| **Data Engineering & Analytics Architecture** | Star-Schema OLAP, In-Process Analytics, Dimensional Modeling, Automated Pipeline Verification | DuckDB, PostgreSQL, SQLite, Supabase |
| **Machine Learning & Predictive Risk** | Supervised Classification, Credit Default Scoring, ROC-AUC Optimization, Feature Engineering | Scikit-Learn (Random Forest, Logistic Regression) |

---

### Featured Projects

#### 1. [Spanish Urban Zoning Burden Analysis](https://github.com/magnumjpg/spanish-urban-zoning-burden-analysis)
**Focus**: Urban Econometrics, Public Choice & Housing Supply Regulation
- An empirical panel study ($N=780$, 15-year horizon, 50 representative Spanish municipalities) investigating how discretionary municipal land-use regulation and bureaucratic permitting bottlenecks restrict housing supply and inflate home prices.
- Estimates structural supply elasticity ($\epsilon_s = 0.31$ under discretionary regimes vs $1.32$ in elastic counterfactuals) and measures welfare deadweight loss at 14.8% of transaction value, calibrated using official 2026 Bank of Spain data (750,000 unit structural deficit).
- **Codebase**: Python, `statsmodels`, Two-Way Fixed Effects panel regressions, 10,000-run Monte Carlo simulations, reproducible Jupyter research notebooks.

#### 2. [B2B Working Capital & CCC Control Tower](https://github.com/magnumjpg/b2b-working-capital-ccc-control-tower)
**Focus**: Corporate Finance, Treasury Analytics & Supply Chain Risk
- An analytical control tower tracking and optimizing Cash Conversion Cycle (CCC), Days Sales Outstanding (DSO), and inventory safety buffers across synthetic ERP transaction records.
- Features Exhaustion (Countback) DSO for unskewed liquidity analysis, a Random Forest credit default risk scoring model (0.92 ROC-AUC), and dual-stochastic 9-cell ABC-XYZ inventory buffer calculations.
- **Codebase**: In-process DuckDB OLAP, Python, Scikit-Learn, Star-Schema dimensional modeling, and automated GitHub Actions CI testing for financial logic.

#### 3. [B2B Revenue Operations & Margin Architecture](https://github.com/magnumjpg/b2b-revenue-operations-analytics)
**Focus**: Strategic Pricing, Commercial Operations & EBITDA Enhancement
- A quantitative framework analyzing pricing realization, invoice-level discounts, and operational margin leakage across simulated B2B commercial transaction data.
- Deconstructs pocket margin waterfalls, maps Stobachoff whale curves to isolate margin-eroding accounts, and models CPQ governance rules driving a projected +791 bps EBITDA improvement.
- **Codebase**: Python, financial waterfall modeling, Pareto analysis, and automated executive reporting pipelines.

#### 4. [La Dehesa del Castrillo — Feasibility & Debt Underwriting](https://github.com/magnumjpg/la-dehesa-financial-due-diligence)
**Focus**: Real Estate Private Equity, Hospitality Due Diligence & Corporate Credit Underwriting
- Quantitative feasibility, operational due diligence, and senior debt underwriting model for a 25-hectare rural hospitality asset in Segovia, Spain (€729,000 CapEx, 70/30 senior debt/equity structure).
- Features dynamic three-statement modeling (P&L, Balance Sheet, Free Cash Flow), empirical INE tourism seasonality calibration, collective agreement labor costing, and 10,000-iteration Monte Carlo stress-testing on debt service coverage (DSCR). Generates institutional multi-tab financial models.
- **Codebase**: Python modular engine (`/src`), automated Pytest test suite (16 tests passed), institutional visualization artifacts, and automated Excel financial model exporter.

---

### Personal Projects & Side Ventures

#### AIchatsplug (Conversational AI Platform for SMBs)
I built AIchatsplug as a self-service tool enabling non-technical business operators to configure and deploy customer support chatbots directly onto their Facebook Messenger and Instagram Direct channels. The core workflow included deep two-way integration with the Google Calendar API to automatically check real-time availability and book appointments without human intervention.

Getting the product to live production required passing rigorous third-party app verification audits: Meta's formal App Review for sensitive Messenger and Instagram Graph API scopes (submitting video walkthroughs, test accounts, and privacy policy compliance) as well as Google's OAuth verification for calendar read/write access. The web interface remains live at [aichatsplug.com](https://aichatsplug.com). After validating product functionality and running initial paid acquisition campaigns on Google Ads and Meta Ads, but I had to ultimatly pause paid advertising because of a lack of capital.

#### Automated Sales Commission & Tier Calculation Engine
A custom backend pipeline designed to solve monthly compensation reconciliation across complex sales structures featuring multi-tiered target thresholds, accelerators, and operational exceptions. The project replaced error-prone manual spreadsheets with an auditable backend engine (FastAPI / Pandas) that processes structured sales exports, generates dispute trails, and computes net payout breakdowns with total transparency.

---

### Contact & Info

- **LinkedIn**: [linkedin.com/in/jaime-pérez-656919237/en](https://www.linkedin.com/in/jaime-p%C3%A9rez-656919237/en)
- **e-mail**: jaimeperezgms@gmail.com
- **Location**: Alcalá de Henares, Spain
