# Jaime Pérez Gómez

Quantitative Analysis | Applied Econometrics | Business Operations & Financial Modeling | Personal Projects

---

### Executive Profile

Quantitative analyst focused on empirical modeling, business operations, and analytical data architectures. My work combines applied econometric methods (panel data, fixed effects, Monte Carlo simulations) with practical data engineering designed for corporate decision-making (DuckDB, dimensional modeling, Python).

- **Focus Areas**: Urban economics and housing supply, pricing and margin optimization, working capital and cash conversion cycle (CCC) analytics, financial risk modeling.
- **Approach**: Reproducible research designs, counterfactual policy simulation, and high-throughput data pipelines.

---

### Core Competencies

| Domain | Methodologies & Frameworks | Tools & Technologies |
| :--- | :--- | :--- |
| **Econometrics & Quantitative Modeling** | Two-Way Fixed Effects (TWFE), Causal Inference, Monte Carlo Simulation, Harberger Deadweight Loss, Tullock Rent-Seeking, Supply Elasticity | Python (`statsmodels`, `linearmodels`, `scipy`), NumPy, Pandas |
| **Corporate Finance & Operations** | Working Capital & CCC Analytics, Countback DSO, Pocket Margin Waterfalls, Stobachoff Whale Curves, CPQ Guardrails | Financial Modeling, Scenario Stress-Testing |
| **Data Engineering & Analytics Architecture** | Star-Schema OLAP, In-Process Analytics, Dimensional Modeling, Automated Pipeline Verification | DuckDB, PostgreSQL, SQLite, Supabase |
| **Machine Learning & Predictive Risk** | Supervised Classification, Credit Default Scoring, ROC-AUC Optimization, Feature Engineering | Scikit-Learn (Random Forest, Logistic Regression) |

---

### Featured Projects

#### 1. [Spanish Urban Zoning Burden Analysis](https://github.com/magnumjpg/spanish-urban-zoning-burden-analysis)
**Domain**: Urban Econometrics, Public Choice & Housing Supply Regulation
- Panel econometric study ($N=780$, 15-year horizon, 50 representative Spanish municipalities) evaluating the causal impact of municipal land-use discretion on housing supply inelasticity and home price inflation.
- Estimates a structural housing supply elasticity of $\epsilon_s = 0.31$ in restrictive regulatory regimes versus $1.32$ in elastic benchmarks, and quantifies welfare deadweight loss (Harberger DWL) at 14.8% of aggregate transaction value. Calibrated against official 2026 Bank of Spain data (750,000 structural housing unit deficit).
- **Stack**: Python, `statsmodels`, Two-Way Fixed Effects, Monte Carlo simulation (10,000 runs), institutional visualization.

#### 2. [B2B Working Capital & CCC Control Tower](https://github.com/magnumjpg/b2b-working-capital-ccc-control-tower)
**Domain**: Corporate Finance, Treasury Analytics & Supply Chain Risk
- Automated analytical control tower to monitor and optimize Cash Conversion Cycle (CCC), Days Sales Outstanding (DSO), and inventory buffers across operational ERP data.
- Implements Countback (Exhaustion) DSO for unskewed liquidity tracking, Random Forest credit default risk scoring achieving 0.92 ROC-AUC, and dual-stochastic 9-cell ABC-XYZ inventory buffer sizing.
- **Stack**: DuckDB, Python, Scikit-Learn, Star-Schema dimensional modeling, automated CI/CD pipeline verifying financial logic.

#### 3. [B2B Revenue Operations & Margin Architecture](https://github.com/magnumjpg/b2b-revenue-operations-analytics)
**Domain**: Strategic Pricing, Commercial Operations & EBITDA Enhancement
- Quantitative framework diagnosing price realization and margin leakage across complex B2B commercial transaction histories.
- Features pocket margin waterfall decomposition, Stobachoff whale curve analysis to isolate margin-eroding accounts, and CPQ governance guardrails modeled to deliver a +791 bps lift in EBITDA margin.
- **Stack**: Python, Financial Waterfall Modeling, Pareto Analytics, Automated Reporting.

---

### Personal Projects & Side Ventures

#### AIchatsplug (Conversational AI Platform for SMBs)
I built AIchatsplug as a self-service tool enabling non-technical business operators to configure and deploy customer support chatbots directly onto their Facebook Messenger and Instagram Direct channels. The core workflow included deep two-way integration with the Google Calendar API to automatically check real-time availability and book appointments without human intervention.

Getting the product to live production required passing rigorous third-party app verification audits: Meta's formal App Review for sensitive Messenger and Instagram Graph API scopes (submitting video walkthroughs, test accounts, and privacy policy compliance) as well as Google's OAuth verification for calendar read/write access. The web interface remains live at [aichatsplug.com](https://aichatsplug.com). After validating product functionality and running initial paid acquisition campaigns on Google Ads and Meta Ads, I paused paid advertising spend to concentrate full-time on quantitative data engineering and analytical modeling.

#### Automated Sales Commission & Tier Calculation Engine
A custom backend pipeline designed to solve monthly compensation reconciliation across complex sales structures featuring multi-tiered target thresholds, accelerators, and operational exceptions. The project replaced error-prone manual spreadsheets with an auditable backend engine (FastAPI / Pandas) that verifies transaction logs, generates dispute trails, and computes net payout breakdowns with total transparency.

---

### Contact & Professional Links

- **LinkedIn**: [linkedin.com/in/jaime-pérez-656919237/en](https://www.linkedin.com/in/jaime-p%C3%A9rez-656919237/en)
- **GitHub**: [github.com/magnumjpg](https://github.com/magnumjpg)
- **Location**: Madrid, Spain
