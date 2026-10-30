# Jaime Pérez Gómez

Financial Analysis & Modeling | Applied Econometrics | Operations & Automation

[Projects](#featured-projects) · [Personal projects](#personal-projects-and-side-ventures) · [Contact](#contact)

---

## Portfolio overview

A set of focused, reproducible models built in Python. Each one answers a single question with public data or with a synthetic dataset that is clearly labeled as such. The goal is not to produce another dashboard: it is to download and validate the inputs, estimate something that can be re-run, and leave a written record of what was tried, what failed and why. Each public repository includes its own tests, figures and a decision or governance record.

---

## Featured projects

1. **[Spain housing supply: Permission Without Construction](https://github.com/magnumjpg/spain-housing-supply)**
   A municipal dataset built from the MIVAU land registry (SIU), the INE urban indicators, tax-record rents and a cross-country benchmark. The project asks whether classifying more land for development actually lowers rents, and measures the pipeline of dwellings that are planned but never built, municipality by municipality. Where the data cannot support a causal claim it says so and stays descriptive.

2. **[Cash conversion cycle: 15 years of SEC filings](https://github.com/magnumjpg/sec-cash-conversion-cycle)**
   A firm-year panel assembled from the SEC's XBRL financial statement datasets, with explicit tag choices and a full attrition record from raw filings to the final sample. It measures how long US listed firms tie up cash in receivables and inventory net of payables, asks whether that cycle is a stable firm characteristic or a fast mean-reverting ratio, and tests whether it travels with profitability and with the 2020 and 2022 shocks.

3. **[Retail demand forecasting](https://github.com/magnumjpg/retail-demand-forecasting)**
   A forecasting exercise on two years of UK online-retail transactions at SKU-week level: several point models and a conformal layer that turns any of them into a distribution. Forecasts are judged by what they would have cost in inventory rather than by accuracy alone, across a grid of lead times and underage-to-holding cost ratios.

4. **[La Dehesa del Castrillo: financial due diligence](https://github.com/magnumjpg/la-dehesa-financial-due-diligence)**
   A feasibility and bank debt underwriting model for a rural hospitality acquisition, built on the promoter's own workbooks together with official occupancy and wage data. It runs three as-is cases, a full cost stack, sources and uses, a 20-year amortizing facility and a computed audit of the model's own rules. It reaches a decline recommendation and documents the audit exceptions as deal findings.

5. **[Omnichannel inventory control tower](https://github.com/magnumjpg/omnichannel-inventory-control-tower)**
   A weekly S&OP engine for a synthetic brand selling through Amazon FBA and a 3PL: demand unconstrained from censored sales, safety stock split across two echelons, purchase orders that respect MOQ, carton and container limits, and removals priced against the aged-inventory fee cliff. The deliverable is the decision logic and an auditable workbook.

---

## Personal projects and side ventures

### AIchatsplug (conversational AI platform for SMBs)

A SaaS platform that lets non-technical businesses set up their own customer-support chatbots on Facebook Messenger, Instagram Direct and their own websites, and connect them to Google Calendar to manage appointments automatically. Taking it to production required passing official security and compliance reviews from both Meta (App Review for the Messenger and Instagram Graph APIs) and Google (OAuth 2.0 and Calendar API access). After validating the product and running initial paid acquisition on Google Ads and Meta Ads, paid advertising was paused to preserve capital.

### Automated sales commission and tier calculation engine

A backend pipeline built to solve monthly compensation reconciliation across complex sales structures with multi-tiered targets, accelerators and operational exceptions. It replaced error-prone manual spreadsheets with an auditable FastAPI and Pandas service that processes structured sales exports, generates dispute trails and computes net payout breakdowns.

---

## Contact

- **LinkedIn**: [linkedin.com/in/jaime-pérez-656919237](https://www.linkedin.com/in/jaime-p%C3%A9rez-656919237/)
- **Email**: [jaimeperezgms@gmail.com](mailto:jaimeperezgms@gmail.com)
- **Location**: Alcalá de Henares, Spain
