<div align="center">

# Dhaval Vibhakar

**Data Scientist · Analytics & Data Engineering · Applied ML / LLM Systems**

<a href="https://github.com/DhavalVibhakar99"><img src="https://readme-typing-svg.demolab.com?font=Inter&weight=600&size=20&duration=2600&pause=900&color=2A78D6&center=true&vCenter=true&width=640&lines=I+build+data+systems+you+can+trust.;Pipelines+that+reconcile+to+the+cent.;Models+validated+like+a+risk+team+would.;LLMs+where+they+help%2C+code+where+it+decides." alt="I build data systems you can trust." /></a>

[![Portfolio](https://img.shields.io/badge/Portfolio-dhaval--vibhakar.lovable.app-111111?style=for-the-badge&logo=googlechrome&logoColor=white)]([https://dhaval-vibhakar.lovable.app](https://dhavalvibhakar.app))
[![LinkedIn](https://img.shields.io/badge/LinkedIn-dhavalvibhakar99-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/dhavalvibhakar99)
[![Email](https://img.shields.io/badge/Email-dhavalvibhakar.data%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:dhavalvibhakar.data@gmail.com)

</div>

---

I turn messy public and financial data into **production-grade pipelines, validated models and decision tools**, and I test every answer against its source, not just the code against itself. M.S. in Information Science (Data Science) from **Pace University**, with 3+ years in technical operations and project coordination before that.

## 🚀 Featured work

### [HeatWatch NYC](https://github.com/DhavalVibhakar99/nyc-heat-energy-pipeline) · *Do energy-inefficient buildings leave tenants cold?*
[![Live dashboard](https://img.shields.io/badge/Live_dashboard-2A78D6?style=flat-square&logo=githubpages&logoColor=white)](https://dhavalvibhakar99.github.io/nyc-heat-energy-pipeline/)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)
![AWS Lambda](https://img.shields.io/badge/AWS_Lambda-FF9900?style=flat-square&logo=awslambda&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

End-to-end **incremental ELT** joining 650K+ NYC 311 heat complaints to Local Law 84 energy benchmarking, refreshed daily.
- **Ingestion:** AWS Lambda with watermark-based incremental extraction, row-count reconciliation and retry/backoff, so a run can never write a partial load; Parquet in S3, loaded into Snowflake through a storage integration
- **Modeling:** dbt staging → intermediate → marts with **unit tests**, data tests and source-freshness checks; point-in-time join of each complaint to the energy score that existed when it was filed
- **Ops:** GitHub Actions CI/CD rebuilds and tests every model, then publishes a public dashboard; failing tests block the deploy
- **Finding:** a Simpson's paradox. Efficiency barely matters pooled, but tracks complaints within smaller and prewar buildings

### [ONRR Revenue Data Migration](https://github.com/DhavalVibhakar99/onrr-revenue-migration) · *$297.5B migrated, $0.00 variance*
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![Delta Lake](https://img.shields.io/badge/Delta_Lake-003366?style=flat-square&logo=delta&logoColor=white)

Federal oil, gas and mineral revenue (2003–present) migrated from CSV into a **Delta Lake star schema** using a **medallion architecture** (bronze/silver/gold) with row-level validation and idempotent loads. **413,554 rows** and **10/10 reconciliation checks**, tied out to published fiscal-year totals across 199 groups in under 3 minutes. AI/BI dashboard with Genie natural-language querying.

### [AML Mule-Account Detection](https://github.com/DhavalVibhakar99/aml-model-validation) · *validated like a bank's model risk team (SR 11-7)*
![LightGBM](https://img.shields.io/badge/LightGBM-02569B?style=flat-square)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

LightGBM vs a tuned rules baseline on IBM synthetic transactions: **10× the rules' recall at 500 alerts**. Frozen holdout, probability calibration, **PSI drift monitoring**, stress testing and leakage tests.

### [Lexorion](https://github.com/DhavalVibhakar99/Lexorion-Cuad) · *contract risk AI that knows when to ask an LLM*
[![Live demo](https://img.shields.io/badge/Live_demo-2A78D6?style=flat-square&logo=googlechrome&logoColor=white)](https://dhavalvibhakar99.github.io/Lexorion-Cuad/demo/)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)

A **recall-first ML cascade** trained on CUAD screens contract clauses and routes only uncertain flags to an LLM for triage: **90% of risky clauses caught** with just **4.4% of decisions** sent to the paid tier. FastAPI inference service and React front end on free-tier cloud.

### More projects

| Project | What it does | Highlights | Links |
|---|---|---|---|
| [KeyClause](https://github.com/DhavalVibhakar99/keyclause) | Which housing laws apply to 500 buildings in CA, NJ and MA | LLM extraction to structured JSON + a deterministic rules engine; 54 validated rules, 95.6% citation coverage | [Demo](https://dhavalvibhakar99.github.io/keyclause/) |
| [Healthcare Billing Intelligence](https://github.com/DhavalVibhakar99/Healthcare-Billing-Intelligence-System) | Anomaly detection on 9M+ CMS Medicare billing records | SQL analytics + natural-language **text-to-SQL** interface | [Demo](https://healthcare-billing-intelligence-system.streamlit.app) |
| [Earnings Sentiment Engine](https://github.com/DhavalVibhakar99/earnings-sentiment-engine) | Does the language in SEC filings move stock prices? | SEC EDGAR extraction, **FinBERT** sentiment, price correlation across 20 companies | [Demo](https://huggingface.co/spaces/dhaval99/earnings-sentiment-engine) |
| [Customer Analytics Dashboards](https://github.com/DhavalVibhakar99/Customer_Analytics_Dashboard) | Call-centre performance, churn risk, workforce diversity | Power BI across 3 business domains | [Repo](https://github.com/DhavalVibhakar99/Customer_Analytics_Dashboard) |

## 🧰 Tech stack

| Area | Tools |
|---|---|
| **Languages** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white) ![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white) |
| **Data engineering** | ![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white) ![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white) ![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white) ![Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white) ![Delta Lake](https://img.shields.io/badge/Delta_Lake-003366?style=flat-square&logo=delta&logoColor=white) ![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black) |
| **Cloud & DevOps** | ![AWS](https://img.shields.io/badge/AWS_(Lambda_·_S3)-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) |
| **ML & AI** | ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white) ![XGBoost](https://img.shields.io/badge/XGBoost-189AB4?style=flat-square) ![LightGBM](https://img.shields.io/badge/LightGBM-02569B?style=flat-square) ![Transformers](https://img.shields.io/badge/Transformers_·_FinBERT-FFD21E?style=flat-square&logo=huggingface&logoColor=black) ![SHAP](https://img.shields.io/badge/SHAP-6E40C9?style=flat-square) ![statsmodels](https://img.shields.io/badge/statsmodels-4051B5?style=flat-square) |
| **LLM apps** | ![OpenRouter](https://img.shields.io/badge/OpenRouter-6566F1?style=flat-square) ![Guardrails](https://img.shields.io/badge/LLM_guardrails-111111?style=flat-square) ![Text-to-SQL](https://img.shields.io/badge/Text--to--SQL-111111?style=flat-square) |
| **Apps & BI** | ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white) ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black) ![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white) ![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white) |
| **Databases** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![Oracle](https://img.shields.io/badge/Oracle_SQL-F80000?style=flat-square&logo=oracle&logoColor=white) ![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white) |

## 🧭 How I work

```text
// Reconcile to the source, not just the run
// Test models like a skeptic would
// Let code decide what code can decide
// Write down why, not just what
```

<div align="center">
<sub>Open to Data Scientist, Analytics Engineer and Data Engineer roles</sub>
</div>
