<a href="https://github.com/DTheDataGuy/the-data-guys-portfolio">
  <img src="https://raw.githubusercontent.com/DTheDataGuy/the-data-guys-portfolio/main/docs/assets/banner.svg" alt="Dei'Marlon Scisney · The Data Guys · Data Engineering Portfolio" width="100%">
</a>

<div align="center">

## Hi, I'm Dei'Marlon "D" Scisney

**Data engineer · President of [The Data Guys™](https://www.thedataguys.org) · Seattle, WA**

I build data systems people can trust and act on: pipelines that quarantine bad rows instead of hiding them, warehouses with tests, and reporting platforms where every number traces back to its source.

[![Portfolio](https://img.shields.io/badge/Portfolio-live%20site-3FB8AF?style=for-the-badge&logo=githubpages&logoColor=white)](https://dthedataguy.github.io/the-data-guys-portfolio/)
[![The Data Guys](https://img.shields.io/badge/The%20Data%20Guys-thedataguys.org-14161A?style=for-the-badge&logo=googlechrome&logoColor=white)](https://www.thedataguys.org)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-deimarlon-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/deimarlon)
[![Email](https://img.shields.io/badge/Email-info%40thedataguys.org-F2C14E?style=for-the-badge&logo=gmail&logoColor=black)](mailto:info@thedataguys.org)

<sub>Data engineer · Ingeniero de datos · Ingénieur de données · Engenheiro de dados · Dateningenieur · データエンジニア · 数据工程师 · مهندس بيانات</sub>

</div>

---

### Start here

| | |
|---|---|
| **[rowgate](https://github.com/DTheDataGuy/rowgate)** <br> Open source · MIT · Python | Data contracts and quality gates for Polars. Quarantines bad rows with the reason for each one, blocks bad batches and writes reports people can read. One dependency. |
| **[the-data-guys-portfolio](https://github.com/DTheDataGuy/the-data-guys-portfolio)** <br> 16 projects · 10 clients | About 33,000 lines of authored code organized by client, with 5 live demos. [Browse it as a website](https://dthedataguy.github.io/the-data-guys-portfolio/). |

### Use my code in 60 seconds

```bash
pip install git+https://github.com/DTheDataGuy/rowgate@v0.1.0
```

```python
import polars as pl, rowgate as rg

contract = rg.Contract(columns={
    "order_id": rg.Column(pl.Int64, required=True, unique=True),
    "amount":   rg.Column(pl.Float64, min=0),
})
result = contract.split(df)   # result.valid loads, result.quarantine says why each row didn't
```

Want to build on it? [Fork rowgate](https://github.com/DTheDataGuy/rowgate/fork), read [CONTRIBUTING](https://github.com/DTheDataGuy/rowgate/blob/main/CONTRIBUTING.md) or start a [discussion](https://github.com/DTheDataGuy/rowgate/discussions). Stars help other data engineers find it.

### Featured work

| Project | What it shows | Try it |
| --- | --- | --- |
| [Seattle Permits Data Platform](https://github.com/DTheDataGuy/the-data-guys-portfolio/tree/main/data-engineering) | 193,747 public permits through a Polars medallion pipeline, a dbt + DuckDB warehouse (61/61 nodes pass), and PySpark and Scala Spark jobs. All four engines agree on 744 result rows with 0 mismatches, and CI runs on every push. | [Code](https://github.com/DTheDataGuy/the-data-guys-portfolio/tree/main/data-engineering) |
| [FIFA World Cup 2026 Seattle Economic Impact](https://github.com/DTheDataGuy/the-data-guys-portfolio/tree/main/clients/regional-sports-commission/wc2026-seattle-economic-dashboard) | Commissioner-facing evidence product with multi-method impact estimates and an evidence register. | [Live demo](https://dthedataguy.github.io/the-data-guys-portfolio/demos/world-cup-economic-dashboard/) |
| [Seattle's World Cup: The Story Behind the Numbers](https://github.com/DTheDataGuy/ssc-worldcup-impact) | Public World Cup impact story with a sourced data bank, infographic builder and press kit. | [Live site](https://dthedataguy.github.io/ssc-worldcup-impact/) |
| [Enterprise WIP Command Center](https://github.com/DTheDataGuy/the-data-guys-portfolio/tree/main/clients/multi-company-construction-enterprise/enterprise-wip-command-center) | Governed work-in-progress reporting for 18+ construction companies: one shared calculation library, reconciliation across Costpoint, HCSS and Procore, and locked month-end versions. | [Code](https://github.com/DTheDataGuy/the-data-guys-portfolio/tree/main/clients/multi-company-construction-enterprise/enterprise-wip-command-center) |
| [RFQ Item Matching Engine](https://github.com/DTheDataGuy/the-data-guys-portfolio/tree/main/clients/aerospace-ndt-distributor/rfq-item-matching-engine) | Python and pandas matching of messy inbound quote requests to a product catalog, with regex extraction, fuzzy matching and unit tests. | [Code](https://github.com/DTheDataGuy/the-data-guys-portfolio/tree/main/clients/aerospace-ndt-distributor/rfq-item-matching-engine) |
| [Ticket Desk](https://github.com/DTheDataGuy/the-data-guys-portfolio/tree/main/clients/regional-heavy-civil-contractor/ticket-desk) | Trucking ticket intake and review for a heavy-civil contractor. | [Live demo](https://dthedataguy.github.io/the-data-guys-portfolio/demos/ticket-desk/) |

### How I work

- **Provenance first.** Every number traces back to a source file, sheet and row, or to a stored response.
- **Quarantine, don't drop.** Bad data is kept with a reason so totals stay auditable.
- **One calculation library.** Server, UI and exports share formulas, so dashboards and reports never disagree.
- **Evidence classes.** Observed data, reported figures, model estimates and plans are labeled separately and never blended.

### Toolkit

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-336791?style=flat-square&logo=postgresql&logoColor=white) ![Apache Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white) ![Scala](https://img.shields.io/badge/Scala-DC322F?style=flat-square&logo=scala&logoColor=white) ![Polars](https://img.shields.io/badge/Polars-CD792C?style=flat-square&logo=polars&logoColor=white) ![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white) ![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black) ![Parquet](https://img.shields.io/badge/Apache_Parquet-50ABF1?style=flat-square&logo=apacheparquet&logoColor=white) ![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white) ![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=flat-square&logo=chartdotjs&logoColor=white) ![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black) ![Power Automate](https://img.shields.io/badge/Power_Automate-0066FF?style=flat-square&logo=powerautomate&logoColor=white)

### Credentials

Formerly an AWS Analytics specialist · MS, Data Engineering · PMP · CISA · Commissioner, Seattle Community Technology Advisory Board · PSBJ 40 Under 40

### Work with me

The Data Guys™ takes on data engineering, data-quality, reporting-platform and economic-impact projects for companies, public agencies and community organizations, wherever they are. Reach out at [info@thedataguys.org](mailto:info@thedataguys.org) or [thedataguys.org](https://www.thedataguys.org).
