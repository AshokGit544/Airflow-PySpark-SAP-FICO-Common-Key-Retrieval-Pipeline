# Airflow PySpark SAP FICO Common Key Retrieval Pipeline

## Overview
This project demonstrates a finance-oriented data engineering pipeline built using Python, PySpark, and Apache Airflow.

The pipeline creates synthetic SAP FICO-style source data, processes it using PySpark, applies data quality checks, builds a common business key for cross-system linking, and generates retrieval-ready output for downstream analytics or AI search use cases.

It also includes an Airflow DAG to orchestrate the pipeline execution.


## Project Objective
The goal of this project is to simulate an enterprise-style finance data pipeline that:

- ingests SAP FICO-style master and transaction datasets
- standardizes and enriches source data
- creates a common business key for unified business linking
- performs data quality validation
- joins invoice, vendor, GL account, cost center, and payment datasets
- produces retrieval-ready and embedding input datasets


## Source Data
The pipeline generates and uses the following source files:

- `vendors.csv`
- `gl_accounts.csv`
- `cost_centers.csv`
- `invoices.csv`
- `payments.csv`

These files are stored under:
data/raw/
