# End-to-End Data Warehouse Pipeline for Flight Analytics using Databricks Lakehouse Platform
**Objective:**
To build a robust and scalable data pipeline for analyzing flight performance metrics by leveraging Databricks Lakehouse Platform with Medallion Architecture, using incremental ingestion, real-time streaming, and dimensional modeling best practices.

**Architecture Overview:**
Data Source: Flight performance datasets (CSV/JSON/Parquet) landing in Azure/ADLS/Blob Storage.

Data Platform: Databricks with Unity Catalog enabled.

Storage Layer: Delta Lake with Bronze → Silver → Gold Medallion architecture.

Ingestion: Real-time via Autoloader with PySpark streaming.

Transformations: Delta Live Tables (DLT) for declarative ETL.

Orchestration: Databricks LakeFlow pipelines and jobs scheduler.

Modeling: Dimensional Data Model (Fact/Dim tables) with DBT for transformation and SCD handling.

| Category       | Tool/Tech                             |
| -------------- | ------------------------------------- |
| Platform       | Databricks, Unity Catalog             |
| Storage        | Delta Lake (Bronze/Silver/Gold)       |
| Ingestion      | Autoloader, PySpark Streaming         |
| Transformation | Delta Live Tables (DLT), PySpark      |
| Orchestration  | LakeFlow Pipelines, Job Scheduler     |
| Modeling       | Dimensional Model (Fact/Dim), DBT     |
| Governance     | Unity Catalog (schemas, data lineage) |
| Languages      | PySpark, SQL, dbt Jinja templating    |
