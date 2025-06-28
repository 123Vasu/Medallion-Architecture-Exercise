# Medallion-Architecture-Exercise
This project demonstrates the Medallion Architecture (Bronze → Silver → Gold) in Databricks using Delta Lake.

## 📁 Architecture Layers

- **Bronze Layer:** Raw ingestion from files like `mote_locs.txt` and `data.txt`. Metadata columns such as `read_time` and `filename` are added.
- **Silver Layer:** (Assumed based on standard architecture) Data cleaning, filtering, and joining to produce refined datasets.
- **Gold Layer:** (Assumed) Aggregated or business-level summaries for analytics/reporting.

## 📌 Key Features

- **Delta Lake Support**: Utilizes Delta format with schema enforcement and evolution.
- **Notebook-based Workflow**: Implemented using a Python notebook in Databricks.
- **Metadata Tracking**: Automatically tracks source file and ingestion time.

## 🚀 Getting Started

1. Import the `.dbc` archive into your Databricks workspace.
2. Open the notebook named **"Medallion Architecture Exercise"**.
3. Execute cells to ingest, process, and persist the datasets in Delta format.

## 📂 Tables Created

- `bronze_mote_locs`
- `bronze_data`

These can be queried using SQL or used as sources for Silver/Gold pipelines.
