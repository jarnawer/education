# Databricks Semantic Model Resources

## Knowledge

- [Databricks docs: Unity Catalog metric views](https://docs.databricks.com/aws/en/business-semantics/metric-views/)
  Primary overview for Metric Views as the core implementation of Unity Catalog business semantics. Use for: understanding the role of Metric Views and how they differ from standard views.
- [Databricks docs: Create and edit metric views](https://docs.databricks.com/aws/en/business-semantics/metric-views/create-edit)
  Official creation guide covering Catalog Explorer, SQL DDL, YAML, prerequisites, fields, measures, and edit flow. Use for: first hands-on Metric View build.
- [Databricks docs: Model metric views](https://docs.databricks.com/aws/en/business-semantics/metric-views/basic-modeling)
  Explains sources, fields, measures, filters, joins, and best practices. Use for: deciding what belongs in the semantic model.
- [Databricks docs: Joins in metric views](https://docs.databricks.com/aws/en/business-semantics/metric-views/joins)
  Explains star schema joins, snowflake joins, join cardinality, `rely`, and one-to-many restrictions. Use for: safely enriching Metric Views with dimension attributes without changing measure grain.
- [Databricks docs: Query metric views](https://docs.databricks.com/aws/en/business-semantics/metric-views/query)
  Shows runtime query patterns, including `MEASURE()`, grouping, filtering, CTE joins, metadata inspection, and downstream consumption. Use for: teaching query semantics.
- [Databricks docs: Metric view tutorial with joins](https://docs.databricks.com/aws/en/business-semantics/metric-views/tpch-example)
  End-to-end TPC-H tutorial with joins, fields, measures, composability, filtered measures, window measures, and agent metadata. Use for: guided build exercises.
- [Databricks docs: Agent metadata in metric views](https://docs.databricks.com/aws/en/business-semantics/agent-metadata)
  Covers display names, synonyms, and formatting for dashboards and Genie. Use for: making semantic models usable by business users and AI tools.
- [Databricks SQL reference: CREATE VIEW](https://docs.databricks.com/aws/en/sql/language-manual/sql-ref-syntax-ddl-create-view)
  SQL syntax reference for standard views and Metric Views using `WITH METRICS LANGUAGE YAML`. Use for: precise DDL syntax and limitations.
- [Databricks SQL reference: `measure` aggregate function](https://docs.databricks.com/aws/en/sql/language-manual/functions/measure)
  Defines how measures are evaluated from Metric Views. Use for: explaining why Metric View queries are not ordinary aggregate queries.
- [Databricks docs: Materialization for metric views](https://docs.databricks.com/aws/en/business-semantics/metric-views/materialization)
  Experimental feature that accelerates Metric Views using materialized views and aggregate-aware query rewriting. Use for: performance architecture and caveats.
- [Databricks docs: Standalone materialized views](https://docs.databricks.com/aws/en/ldp/dbsql/materialized)
  Official guide to standalone Materialized Views, refresh modes, incremental refresh, costs, serverless pipelines, and limitations. Use for: choosing MVs for ETL and dashboard acceleration.
- [Databricks SQL reference: CREATE MATERIALIZED VIEW](https://docs.databricks.com/aws/en/sql/language-manual/sql-ref-syntax-ddl-create-materialized-view)
  Syntax and permissions reference for materialized views, including schedules, `TRIGGER ON UPDATE`, row filters, masks, and limitations. Use for: exact DDL examples.
- [Databricks docs: Dashboards](https://docs.databricks.com/aws/en/dashboards/)
  Entry point for AI/BI dashboards, authoring, sharing, automation, and monitoring. Use for: dashboard capability map.
- [Databricks docs: Create and manage dashboard datasets](https://docs.databricks.com/aws/en/dashboards/manage/data-modeling/datasets)
  Explains dashboard datasets, Metric View usage, SQL datasets, security concerns, and export to Metric Views or Materialized Views. Use for: dashboard data modeling lessons.
- [Databricks docs: Dashboard custom calculations](https://docs.databricks.com/aws/en/dashboards/manage/data-modeling/custom-calculations/)
  Explains dashboard-scoped calculated measures and dimensions, including when to promote reusable calculations to Unity Catalog Metric Views. Use for: deciding what can stay local to a dashboard versus what belongs in a governed Metric View.
- [Databricks docs: Dataset optimization and caching](https://docs.databricks.com/aws/en/dashboards/caching)
  Covers browser-side processing thresholds, backend queries, 24-hour dashboard cache, query result cache, schedules, and credentials. Use for: freshness and performance lessons.
- [Databricks docs: Create a dashboard tutorial](https://docs.databricks.com/aws/en/dashboards/tutorials/create-dashboard)
  Official hands-on dashboard tutorial using sample data. Use for: beginner dashboard workflow, skipping general SQL basics as needed.
- [Databricks docs: Genie Spaces with dashboards](https://docs.databricks.com/aws/en/dashboards/genie-spaces)
  Explains dashboard companion Genie Spaces, credential behavior, dataset exposure, and limitations. Use for: AI/BI governance and semantic metadata lessons.

## Wisdom (Communities)

- [Databricks Community](https://community.databricks.com/)
  Official Databricks community forum. Use for: product-specific edge cases, release behavior, and practitioner answers.
- [Databricks Community: Data Engineering discussions](https://community.databricks.com/t5/data-engineering/bd-p/data-engineering)
  High-relevance forum area for lakehouse engineering and SQL warehouse operational questions. Use for: real-world refresh, cost, and deployment tradeoffs.
- [Databricks Events and User Groups](https://www.databricks.com/events)
  Official event directory for webinars and meetups. Use for: practitioner demos and release-era context.

## Gaps

- Need targeted examples from your own business domain or datasets once you choose a sample use case.
- Need current Databricks release-note tracking for Metric View feature availability and experimental materialization behavior before production recommendations.
