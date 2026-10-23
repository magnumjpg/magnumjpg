# Jaime Pérez Gómez

Quantitative Analysis | Applied Econometrics | Business Operations & Financial Modeling | Personal Projects

---

### Portfolio Overview

This GitHub workspace compiles end-to-end quantitative research, financial operations frameworks, and analytical engineering systems. The repositories hosted here focus on translating real-world operational bottlenecks, regulatory friction, and corporate finance dynamics into reproducible data pipelines, econometric estimations, and executive decision models.

Each project is designed with modular architectures, strict separation of concerns, and comprehensive documentation covering empirical methodologies, financial logic, and technical implementations.

---

### Core Competencies & Frameworks

| Domain | Methodologies & Frameworks | Tools & Technologies |
| :--- | :--- | :--- |
| **Econometrics & Quantitative Modeling** | Two-Way Fixed Effects (TWFE), Causal Inference, Monte Carlo Simulation, Harberger Deadweight Loss, Tullock Rent-Seeking, Supply Elasticity | Python (`statsmodels`, `linearmodels`, `scipy`), NumPy, Pandas |
| **Corporate Finance & Operations** | Working Capital & CCC Analytics, Countback DSO, Pocket Margin Waterfalls, Stobachoff Whale Curves, CPQ Guardrails | Financial Modeling, Scenario Stress-Testing |
| **Data Engineering & Analytics Architecture** | Star-Schema OLAP, In-Process Analytics, Dimensional Modeling, Automated Pipeline Verification | DuckDB, PostgreSQL, SQLite, Supabase |
| **Machine Learning & Predictive Risk** | Supervised Classification, Credit Default Scoring, ROC-AUC Optimization, Feature Engineering | Scikit-Learn (Random Forest, Logistic Regression) |

---

### Featured Repositories

#### 1. [Spanish Urban Zoning Burden Analysis](https://github.com/magnumjpg/spanish-urban-zoning-burden-analysis)
**Focus**: Urban Econometrics, Public Choice & Housing Supply Regulation
- An empirical panel study ($N=780$, 15-year horizon, 50 representative Spanish municipalities) investigating how discretionary municipal land-use regulation and bureaucratic permitting bottlenecks restrict housing supply and inflate home prices.
- Estimates structural supply elasticity ($\epsilon_s = 0.31$ under discretionary regimes vs $1.32$ in elastic counterfactuals) and measures welfare deadweight loss at 14.8% of transaction value, calibrated using official 2026 Bank of Spain data (750,000 unit structural deficit).
- **Codebase**: Python, `statsmodels`, Two-Way Fixed Effects panel regressions, 10,000-run Monte Carlo simulations, reproducible Jupyter research notebooks.

#### 2. [B2B Working Capital & CCC Control Tower](https://github.com/magnumjpg/b2b-working-capital-ccc-control-tower)
**Focus**: Corporate Finance, Treasury Analytics & Supply Chain Risk
- An analytical control tower tracking and optimizing Cash Conversion Cycle (CCC), Days Sales Outstanding (DSO), and inventory safety buffers across enterprise ERP transaction histories.
- Features Exhaustion (Countback) DSO for unskewed liquidity analysis, a Random Forest credit default risk scoring model (0.92 ROC-AUC), and dual-stochastic 9-cell ABC-XYZ inventory buffer calculations.
- **Codebase**: In-process DuckDB OLAP, Python, Scikit-Learn, Star-Schema dimensional modeling, and automated GitHub Actions CI testing for financial logic.

#### 3. [B2B Revenue Operations & Margin Architecture](https://github.com/magnumjpg/b2b-revenue-operations-analytics)
**Focus**: Strategic Pricing, Commercial Operations & EBITDA Enhancement
- A quantitative framework analyzing pricing realization, invoice-level discounts, and operational margin leakage across complex commercial transaction records.
- Deconstructs pocket margin waterfalls, maps Stobachoff whale curves to isolate margin-eroding accounts, and models CPQ governance rules driving a projected +791 bps EBITDA improvement.
- **Codebase**: Python, financial waterfall modeling, Pareto analysis, and automated executive reporting pipelines.

---

### Personal Projects & Side Ventures

#### AIchatsplug (Conversational AI Platform for SMBs)
I built AIchatsplug as a self-service tool enabling non-technical business operators to configure and deploy customer support chatbots directly onto their Facebook Messenger and Instagram Direct channels. The core workflow included deep two-way integration with the Google Calendar API to automatically check real-time availability and book appointments without human intervention.

Getting the product to live production required passing rigorous third-party app verification audits: Meta's formal App Review for sensitive Messenger and Instagram Graph API scopes (submitting video walkthroughs, test accounts, and privacy policy compliance) as well as Google's OAuth verification for calendar read/write access. The web interface remains live at [aichatsplug.com](https://aichatsplug.com). After validating product functionality and running initial paid acquisition campaigns on Google Ads and Meta Ads, I paused paid advertising spend to concentrate full-time on quantitative data engineering and analytical modeling.

#### Automated Sales Commission & Tier Calculation Engine
A custom backend pipeline designed to solve monthly compensation reconciliation across complex sales structures featuring multi-tiered target thresholds, accelerators, and operational exceptions. The project replaced error-prone manual spreadsheets with an auditable backend engine (FastAPI / Pandas) that verifies transaction logs, generates dispute trails, and computes net payout breakdowns with total transparency.

---

### Professional Links

- **LinkedIn**: [linkedin.com/in/jaime-pérez-656919237/en](https://www.linkedin.com/in/jaime-p%C3%A9rez-656919237/en)
- **GitHub**: [github.com/magnumjpg](https://github.com/magnumjpg)
- **Location**: Madrid, Spain
