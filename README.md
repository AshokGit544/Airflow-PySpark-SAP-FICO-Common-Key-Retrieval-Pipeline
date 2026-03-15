# Airflow PySpark SAP FICO Common Key Retrieval Pipeline

This project shows how SAP FICO-style finance data can be processed in a simple enterprise-style pipeline using PySpark and Airflow.

The main idea of this project is to take finance data from separate source files, clean it, connect it using a common business key, check data quality issues, and prepare the data for retrieval and embedding use cases.

## What this project does

In this project, I created a simple pipeline that:

- loads SAP FICO-style source data
- cleans and standardizes the records
- creates a common business key
- joins separated datasets into one integrated finance view
- checks for data quality issues
- builds retrieval-ready text
- prepares embedding input
- shows how Airflow can automate the job flow

## Why this project is important

In large companies, data is usually stored in separate systems.  
Even when the data is separated, business users still need one integrated view.

This project shows how to:

- keep source data separate
- create a common key
- connect the data into one business view
- apply clean rules
- prepare the final data for AI and retrieval use cases

This is useful for enterprise environments where SAP FICO and other business systems need to support reporting, search, and AI-ready workflows.

## Main topics covered

- PySpark
- Apache Airflow
- SAP FICO-style data
- Common key modeling
- Integrated data view
- Data quality checks
- Retrieval-ready output
- Embedding input preparation
- Pipeline automation

## Project structure

``` id="vt5f5r"
Airflow-PySpark-SAP-FICO-Common-Key-Retrieval-Pipeline/
│
├── dags/
│   └── sap_fico_common_key_retrieval_dag.py
│
├── data/
│   ├── raw/
│   │   ├── vendors.csv
│   │   ├── gl_accounts.csv
│   │   ├── cost_centers.csv
│   │   ├── invoices.csv
│   │   └── payments.csv
│   │
│   └── output/
│       ├── integrated_finance_view.csv
│       ├── data_quality_issues.csv
│       ├── retrieval_ready_documents.csv
│       └── embedding_input.csv
│
├── pyspark_job.py
├── requirements.txt
├── README.md
└── .gitignore
