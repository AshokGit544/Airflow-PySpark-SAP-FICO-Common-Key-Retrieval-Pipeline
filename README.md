# Airflow → Databricks → PySpark SAP FICO Common Key Retrieval Pipeline

This project demonstrates an enterprise data engineering pipeline where Apache Airflow orchestrates a Databricks PySpark job to process SAP FICO-style financial data and prepare it for AI and retrieval use cases.


## 🚀 What this project does

* Loads SAP FICO-style source data (vendors, invoices, payments, etc.)
* Cleans and standardizes records
* Creates a **common business key** to connect datasets
* Integrates data into a unified finance view
* Performs **data quality checks**
* Generates **retrieval-ready text**
* Prepares **embedding input for AI/LLM use cases**
* Uses **Airflow to trigger Databricks jobs**


## 🏗️ Architecture

Airflow triggers Databricks using API → Databricks runs PySpark → outputs AI-ready datasets



Airflow DAG
    ↓
Databricks Job Trigger (API)
    ↓
PySpark Processing
    ↓
Integrated Data + AI-ready Outputs


## 🎯 Why this project is important

* Enterprise data (SAP FICO) is distributed across systems
* Requires **common-key-based integration**
* Needs **clean, reliable, and AI-ready data**

This project shows:

* Data integration using business keys
* Data quality validation
* Preparation for **RAG / LLM workflows**
* Real-world orchestration using Airflow + Databricks


## 📂 Project Structure

Airflow-PySpark-SAP-FICO-Common-Key-Retrieval-Pipeline/
│
├── dags/
│   └── sap_fico_airflow_to_databricks_trigger.py
│
├── data/
│   ├── raw/
│   └── output/
│
├── pyspark_job_databricks.py
├── requirements.txt
└── README.md

## ⚙️ Pipeline Flow

1. Airflow triggers Databricks job
2. PySpark processes and integrates data
3. Outputs generated:

   * Integrated finance view
   * Data quality issues
   * Retrieval-ready documents
   * Embedding input

## 📊 Output Files

* `integrated_finance_view.csv` → unified dataset
* `data_quality_issues.csv` → validation issues
* `retrieval_ready_documents.csv` → search-ready text
* `embedding_input.csv` → AI embedding input

## 🤖 AI / LLM Use Case

* Semantic search
* Retrieval-Augmented Generation (RAG)
* Embedding-based similarity search

## 🧩 Technologies

* Python, PySpark
* Apache Airflow
* Databricks
* Pandas

## 🔥 Key Highlight

End-to-end pipeline:
Airflow (orchestration) → Databricks (processing) → PySpark (transformation) → AI-ready data

## ✅ Conclusion

This project shows how enterprise finance data can be transformed into an integrated, validated, and AI-ready format using modern data engineering architecture.
