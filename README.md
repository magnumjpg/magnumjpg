# Jaime Pérez Gómez

Quantitative analysis · applied econometrics · operations and financial modelling

I build small, reproducible models that answer one question each, using public data or a clearly labelled synthetic catalogue. Every project ships its own tests, figures and a written decision record, and every headline number is a field of that project's `outputs/results.json` or equivalent artefact — not a figure typed into the README by hand.

The rule I work to: state the question before looking, report the result whether or not it is the one I wanted, and keep the failures in the write-up.

---

## The five projects

### 1. [Permission Without Construction](https://github.com/magnumjpg/spain-housing-supply) — housing supply in Spain

**Question.** Does classifying more land for development lower rents?

**Data.** MIVAU SIU (5,898 municipalities), INE Urban Indicators, SERPAVI, OECD and Eurostat comparisons; 431-municipality matched sample.

**Finding.** The rent link does not survive urbanisation controls and province fixed effects: the non-urbanizable share is associated with −4.6% rents per SD (p = 0.21), development land with +1.5% (p = 0.45). What the data do show is a paper pipeline: **3.49 M of 5.17 M planned dwellings (67.5%) are unbuilt**, and in the 359 municipalities with positive net additions the 3.17 M pending equal **45.7 years** of construction at the 2023–2025 rate. Spain permits **2.64** dwellings per 1,000 (28th of 33; European median 4.62).

**Caveat.** The rent result is a null, not proof that regulation has no effect; the years figure is a sample-conditional description with two filters that bias in opposite directions, not a forecast or a bound. 41 tests, 10 figures.

---

### 2. [Cash Conversion and Resilience](https://github.com/magnumjpg/sec-cash-conversion-cycle) — 15 years of SEC filings

**Question.** How long is the cash conversion cycle of US listed firms, is it a firm trait, and does it predict resilience?

**Data.** SEC XBRL Financial Statement Data Sets, FY2010–2024: **25,341 firm-years / 3,158 firms**, with tag-level provenance and a full attrition funnel.

**Finding.** Median CCC **74.97 days** (median of firm-level medians 66.34). It is mostly a firm trait — 64.2% of variance between firms, only 6.0% between industries — and persistent, but persistence is a **range (0.27–0.69)** depending on the estimator. The CCC–ROA association is **positive** (β = +0.000139, significant in 7 of 11 main specifications), which contradicts the simple "shorter CCC is better" story.

**Caveat.** The level is tag-sensitive (11.0% of rows use an AP fallback that cuts the median), the sample is listed US filers, and the design is descriptive, not causal. 30 tests, 6 figures.

---

### 3. [Forecasting Sparse Demand](https://github.com/magnumjpg/retail-demand-forecasting) — UCI Online Retail II

**Question.** Do calibrated probabilistic SKU forecasts reduce inventory cost relative to point forecasts?

**Data.** 104 weeks of UK online-retail transactions, 972,068 cleaned line items, **3,186 SKUs**, three rolling origins, seven point models plus a shared conformal layer.

**Finding.** At the central newsvendor case (4-week lead time, cost ratio 9), ordering the 90th percentile of SES cuts total cost by **23.82%** versus the best simple point rule (95% bootstrap CI 21.20–26.18%; one-sided *p* < 0.0001) and by 18.62% versus the cheapest point rule in that cell. For SES the saving is positive in **12 of 12** lead-time × cost-ratio cells (1.67–48.81%), and the best quantile model per cell ranges from 2.43% to 48.81%.

**Caveat.** The 23.82% is an **ex-post** model choice inside the central cell and the CI is conditional on it; at cost ratio 1 the quantile policy **loses to the cheapest point rule** at every lead time; there is no stockout data and costs are assumptions. 24 tests, 7 figures.

---

### 4. [La Dehesa del Castrillo](https://github.com/magnumjpg/la-dehesa-financial-due-diligence) — hospitality due diligence

**Question.** Is a 25-hectare rural estate in Segovia a fundable investment at official occupancy, at the promoter's numbers, or under professional management?

**What it is.** A three-statement model of three as-is cases (promoter, INE market, management), a full cost stack, sources and uses, a 20-year amortising facility, a live-formula Excel workbook, a computed 16-rule audit and 74 tests.

**Finding.** Management revenue €154,548 and EBITDA €24,280, but minimum DSCR **1.15x** against a 1.25x covenant; the market case is insolvent at official INE occupancy; the promoter case is the only one with a positive equity IRR on exit (12.12%) and is cash-negative in Years 1–2. CapEx is €1,050,100 with **49.6% cash equity**. The audit passes 9 rules, reports 1 as not applicable, and fails 5 materially and 1 as a warning - all five material failures are deal findings, not formula errors.

**Caveat.** The promoter case is a **re-modelling calibrated to the presentation headline (€86,275 / €11,297), not a replication**: the two source workbooks contain four mutually inconsistent Year-1 revenues and two EBITDAs, and the README reconciles them. The report is a diligence artefact on a real project, not an investment recommendation.

---

### 5. [Omnichannel Inventory Control Tower](https://github.com/magnumjpg/omnichannel-inventory-control-tower) — S&OP automation

**Question.** Given right-censored sales, two fulfilment echelons, MOQ/carton/container constraints and Amazon's aged-inventory and low-inventory fees, what should a small brand actually ship, hold and remove this week?

**What it is.** A deterministic weekly S&OP engine for a **synthetic** 160-SKU travel brand (seed 42, 365 days): a censoring-aware demand ladder scored on nine walk-forward cutoffs, a two-echelon safety-stock split behind a 28-day FBA fee shield, a reconciled factory PO and 20′ container, and removal payback against the aged-inventory cliff. Output: a six-tab Excel 365 workbook with **8,048 live formulas**, an executive briefing and 65 tests.

**Finding in the current snapshot.** 11,450 units / 147 cartons from 3PL to FBA, 38,750 units / 461 cartons / 26.910 CBM from the factory, a 28.770 CBM container at 99.9% fill, **$3,442** of 30-day fee exposure, and two economically justified removals.

**Caveat.** Every transaction and balance is synthetic and clearly labelled as such; the value is in the decision logic and the auditable workbook, not in the market realism of the catalogue. The estimator is deterministic, not ML, because the project's face is process automation. 65 tests.

---

## How they are built

| Project | Data | Tests | Main artefact |
|---|---|---:|---|
| Spain housing supply | Official (MIVAU, INE, SERPAVI, OECD, Eurostat) | 41 | `outputs/results.json`, 14 tables, 10 figures |
| SEC cash conversion | Official SEC XBRL filings | 30 | `outputs/results.json`, `validation.json`, 17 tables |
| Retail demand forecasting | Public UCI Online Retail II | 24 | `outputs/results.json`, 8 tables, 7 figures |
| La Dehesa due diligence | Promoter workbooks + INE + convenio | 74 | 13-tab live Excel, audit JSON, 8 figures |
| Inventory control tower | Synthetic catalogue (seed 42) | 65 | 6-tab live Excel, briefing, processed CSV/JSON |

The three new analyses also carry the same process documents: `DECISIONS.md` (each choice, the alternatives rejected, the cost), `ANALYSIS_LOG.md` (what broke and when it was reframed), `RED_TEAM.md` (the hostile referee, answered or conceded) and `LIMITATIONS.md` (what the design cannot establish). La Dehesa adds a `RED_TEAM.md` and a `MODEL_GOVERNANCE.md` pack. All five run their test suite in GitHub Actions on every push to `main`.

No project is a flagship. They are five different methods applied to five different questions. In the three new analyses, two of the expected answers failed and are documented with the same care as the results.

---

## Resumen en español

**01 — Permiso sin construcción.** Con datos del SIU (5.898 municipios), del INE y del SERPAVI, clasificar más suelo no se traduce en alquileres más bajos una vez se controla la urbanización y la provincia. Lo que sí aparece es una cartera de papel: **3,49 de 5,17 millones de viviendas planificadas (67,5%) no se han construido**, equivalentes a **45,7 años** de obra al ritmo de 2023–2025. España licencia 2,64 viviendas por 1.000 habitantes (28ª de 33). El nulo de alquileres es un límite del diseño, no una prueba de ausencia de efecto.

**02 — Circulante y resistencia.** Panel de 25.341 empresas-año (3.158 empresas, 2010–2024) desde los ficheros XBRL de la SEC. El ciclo de conversión de caja mediano es de **74,97 días**, sobre todo un rasgo de empresa (64,2% de la varianza), persistente pero con un rango de **0,27–0,69** según el estimador. Su asociación con la rentabilidad es **positiva**, al contrario de la historia habitual, y el nivel es sensible al tag de cuentas a pagar.

**03 — Previsión de demanda dispersa.** 104 semanas de un minorista online británico, 3.186 SKU y tres orígenes móviles. Pedir el cuantil 0,90 reduce el coste un **23,82%** frente a la mejor regla puntual simple en el caso central, y para SES la mejora es positiva en las 12 celdas de duración × ratio de coste (1,67–48,81%), con el mejor modelo por celda entre el 2,43% y el 48,81%, pero el modelo se elige ex post y con ratio de coste 1 la política por cuantiles pierde frente a la regla puntual más barata.

**04 — La Dehesa del Castrillo.** Modelo de tres estados para tres casos as-is. La gestión llega a 1,15x de DSCR mínimo frente a un covenant de 1,25x; el caso de mercado es insolvente con la ocupación oficial del INE; el promotor es el único con TIR de equity positiva en la salida (12,12%) y tiene caja negativa en los Años 1–2. La auditoría de 16 reglas pasa 9, declara 1 no aplicable y falla 5 materialmente y 1 como aviso. El caso promotor está **re-modelado** sobre el titular de la presentación (86.275 € / 11.297 €), no replicado: los libros fuente contienen cuatro ingresos del Año 1 incompatibles entre sí.

**05 — Torre de control de inventario.** Motor determinista de S&OP para una marca **sintética** de 160 SKU (semilla 42, 365 días): demanda des-censurada, reparto FBA/3PL con escudo de tarifas, PO de fábrica y contenedor 20′ conciliados, y payback de retirada frente al acantilado de inventario envejecido. En el snapshot actual: 11.450 u / 147 cartones al FBA, 38.750 u / 461 cartones de fábrica, contenedor al 99,9% y 3.442 $ de exposición a tarifas a 30 días. Todo el catálogo es sintético y así se declara.

---

## Side ventures

**AIchatsplug** — a SaaS that let non-technical businesses run customer-support chatbots on Messenger, Instagram and their own sites, with Google Calendar appointment booking. Took it through Meta App Review and Google OAuth verification, validated the product and ran paid acquisition on Google and Meta Ads; paused paid advertising for lack of capital.

**Automated Sales Commission Engine** — a FastAPI/Pandas backend that reconciles multi-tier commission plans with accelerators and exceptions, replacing manual spreadsheets with an auditable engine that produces dispute trails and net payout breakdowns.

---

## Contact

- **LinkedIn:** [jaime-pérez-656919237](https://www.linkedin.com/in/jaime-p%C3%A9rez-656919237/en)
- **Email:** jaimeperezgms@gmail.com
- **Location:** Alcalá de Henares, Spain
