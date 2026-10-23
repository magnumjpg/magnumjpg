# Jaime Pérez Gómez

Quantitative Analysis | Applied Econometrics | Business Operations & Financial Modeling | Personal Projects

---

### Executive Profile

Analista cuantitativo enfocado en modelado empírico, operaciones de negocio y arquitecturas analíticas de datos. Mi trabajo combina análisis econométrico riguroso (datos de panel, efectos fijos, simulaciones Monte Carlo) con ingeniería de datos orientada a la toma de decisiones empresariales (DuckDB, modelado dimensional, Python).

- **Áreas de interés**: Econometría urbana, pricing y optimización de márgenes, gestión de capital circulante (Working Capital / CCC), modelado de riesgo financiero.
- **Enfoque técnico**: Diseños reproducibles, simulación de escenarios contrafactuales y pipelines de datos de alto rendimiento.

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
- Estudio econométrico de panel ($N=780$, horizonte de 15 años, 50 municipios españoles) que evalúa el impacto causal de la discrecionalidad urbanística municipal sobre la inelasticidad de la oferta y los precios residenciales.
- Estima una elasticidad de oferta estructural de $\epsilon_s = 0.31$ en municipios restrictivos frente al $1.32$ en entornos elásticos, cuantificando una pérdida de bienestar (Harberger Deadweight Loss) del 14.8% del valor transaccionado, calibrado con datos oficiales del Banco de España de 2026 (déficit de 750.000 viviendas).
- **Stack**: Python, `statsmodels`, Two-Way Fixed Effects, simulación Monte Carlo (10.000 iteraciones), visualización institucional.

#### 2. [B2B Working Capital & CCC Control Tower](https://github.com/magnumjpg/b2b-working-capital-ccc-control-tower)
**Domain**: Corporate Finance, Treasury Analytics & Supply Chain Risk
- Torre de control analítica para monitorizar y optimizar el Ciclo de Conversión de Efectivo (CCC), Días de Cobro (DSO) e inventarios a partir de datos operacionales.
- Implementa cálculo de DSO por agotamiento (*Countback*), modelos de Machine Learning (Random Forest) para scoring de impago crediticio con AUC de 0.92, y matrices estocásticas ABC-XYZ para dimensionamiento de stock de seguridad.
- **Stack**: DuckDB, Python, Scikit-Learn, modelado dimensional Star-Schema, CI/CD con validación de lógica financiera.

#### 3. [B2B Revenue Operations & Margin Architecture](https://github.com/magnumjpg/b2b-revenue-operations-analytics)
**Domain**: Strategic Pricing, Commercial Operations & EBITDA Enhancement
- Marco cuantitativo de diagnóstico de fugas de margen y realización de precios en transacciones comerciales complejas B2B.
- Desarrolla el desglose analítico en cascada (*pocket margin waterfall*), curvas de Stobachoff para identificar clientes destructores de margen y reglas de gobernanza comercial con un impacto potencial de +791 bps en margen EBITDA.
- **Stack**: Python, modelado financiero de cascada de precios, análisis de Pareto, automatización de reporting.

---

### Personal Projects & Side Ventures

#### AIchatsplug (Plataforma Conversacional de IA para Pymes)
Desarrollé AIchatsplug como una solución para que pequeños negocios y operadores sin conocimientos de programación pudieran crear asistentes conversacionales inteligentes y desplegarlos directamente en sus canales de Facebook Messenger e Instagram Direct. El sistema se integraba de forma bidireccional con la API de Google Calendar para gestionar citas de clientes, comprobar huecos libres y registrar reservas de manera autónoma.

Llevar el proyecto a producción exigió superar las revisiones oficiales de permisos sensibles de Meta (proceso completo de App Review para Messenger e Instagram Graph APIs, preparando grabaciones en vídeo, flujos de prueba y cumplimiento de políticas de privacidad) y la verificación de OAuth de Google para el acceso a calendarios. El frontend continúa desplegado y activo en [aichatsplug.com](https://aichatsplug.com). Tras validar técnicamente la plataforma y realizar campañas iniciales de adquisición en Google Ads y Meta Ads, pausé el gasto en paid media para enfocarme al 100% en la parte técnica y analítica de datos.

#### Motor de Automatización de Comisiones Comerciales
Proyecto enfocado en resolver el cálculo mensual de liquidaciones en esquemas de incentivos comerciales con múltiples tramos, objetivos escalonados y excepciones operativas. El sistema reemplaza hojas de cálculo manuales por un backend estructurado (FastAPI / Pandas) que valida los registros de ventas, audita incidencias y calcula las liquidaciones de forma transparente.

---

### Contact & Professional Links

- **LinkedIn**: [linkedin.com/in/jaime-pérez-656919237/en](https://www.linkedin.com/in/jaime-p%C3%A9rez-656919237/en)
- **GitHub**: [github.com/magnumjpg](https://github.com/magnumjpg)
- **Location**: Madrid, Spain
