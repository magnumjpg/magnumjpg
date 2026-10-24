# Jaime Pérez Gómez

Quantitative Analysis | Applied Econometrics | Business Operations & Financial Modeling | Personal Projects

---

### Portfolio Overview

This repository serves as an archive of the code and analytical projects I developed using AI over the past year. These projects have been useful for practical learning, technical experimentation, and putting the finance, economics, and operations concepts from my degree into practice. The projects use public datasets (such as the Bank of Spain and INE) and realistic business simulations.

---

### Core Stack & Focus Areas

| Area | What I Work On | Tools |
| :--- | :--- | :--- |
| **Econometrics & Data Analysis** | Panel data regressions (Fixed Effects), supply elasticity, Monte Carlo simulations | Python (`statsmodels`, `scipy`), Pandas, NumPy |
| **Finance & Operations** | 3-statement financial modeling, Working Capital (CCC/DSO), B2B pricing & margin analysis | Advanced Excel, VBA, OpenPyXL |
| **Data & Automation** | Local analytical databases, data cleaning pipelines, API integrations, predictive scoring | DuckDB, SQLite, Supabase, Scikit-Learn |

---

### Featured Projects

#### 1. [Spanish Urban Zoning Burden Analysis](https://github.com/magnumjpg/spanish-urban-zoning-burden-analysis)
An econometric study ($N=780$, 50 Spanish municipalities over 15 years) analyzing how local land-use regulations and slow building permits restrict housing supply and drive up prices.
- Estimates housing supply elasticity ($\epsilon_s = 0.31$ in strict municipalities vs. $1.32$ in flexible ones) and models the economic loss using Bank of Spain housing deficit data.
- **Tech**: Python, `statsmodels` (Two-Way Fixed Effects), Monte Carlo simulation, Jupyter Notebooks.

#### 2. [B2B Working Capital & CCC Control Tower](https://github.com/magnumjpg/b2b-working-capital-ccc-control-tower)
A tool designed to track and optimize Cash Conversion Cycle (CCC), Days Sales Outstanding (DSO), and inventory safety stock across B2B transaction records.
- Calculates real collection times (Countback DSO), scores client default risk using a Random Forest model (0.92 ROC-AUC), and segments inventory buffers (ABC-XYZ).
- **Tech**: Python, DuckDB, Scikit-Learn, automated testing with GitHub Actions.

#### 3. [B2B Revenue Operations & Margin Analysis](https://github.com/magnumjpg/b2b-revenue-operations-analytics)
An analysis of B2B invoicing and discounts to find where a company is losing margin on its sales.
- Deconstructs pocket margin waterfalls, maps Stobachoff whale curves to isolate margin-eroding accounts, and models CPQ governance rules driving a projected +791 bps EBITDA improvement.
- **Tech**: Python, Pareto & margin waterfall modeling, automated reporting.

#### 4. [La Dehesa del Castrillo — Financial Feasibility Model](https://github.com/magnumjpg/la-dehesa-financial-due-diligence)
A complete financial viability and debt model for a rural hospitality project in Segovia, Spain (€729k CapEx, 70/30 debt-to-equity).
- Connects a dynamic 3-statement model (P&L, Balance Sheet, Cash Flow) with real INE tourism seasonality data, Spanish labor costs, and Monte Carlo stress tests on debt coverage (DSCR).
- **Tech**: Python, `pytest`, and an automated exporter that builds the multi-tab Excel financial model.
---

### Personal Projects & Side Ventures

#### AIchatsplug (Conversational AI Platform for SMBs)
A Saas platform that enables non-technical businesses to set up their own customer support AI chatbots on Facebook Messenger, Instagram Direct, and their own websites and also they could connect their chatbot to Google Calendar to manage appointments automatically.
Taking the product to production required passing official security and compliance reviews from both Meta (App Review for Messenger/Instagram Graph APIs) and Google (OAuth2.0 and API Calendar access). After validating product functionality and running initial paid acquisition campaigns on Google Ads and Meta Ads, I ultimately had to pause paid advertising due to a lack of capital.

#### Automated Sales Commission & Tier Calculation Engine
A custom backend pipeline designed to solve monthly compensation reconciliation across complex sales structures featuring multi-tiered target thresholds, accelerators, and operational exceptions. The project replaced error-prone manual spreadsheets with an auditable backend engine (FastAPI / Pandas) that processes structured sales exports, generates dispute trails, and computes net payout breakdowns with total transparency.

---

### Contact & Info

- **LinkedIn**: [linkedin.com/in/jaime-pérez-656919237/en](https://www.linkedin.com/in/jaime-p%C3%A9rez-656919237/en)
- **e-mail**: jaimeperezgms@gmail.com
- **Location**: Alcalá de Henares, Spain
