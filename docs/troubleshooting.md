## PySpark PATH_NOT_FOUND Issue

### Problem
PySpark job failed because it could not find input files.

### Root Cause
Used relative paths:
base_path = "data/raw"

Spark looked in the wrong directory.

Fix

Used project root:

project_root = "Airflow-PySpark-SAP-FICO-Common-Key-Retrieval-Pipeline"
base_path = f"{project_root}/data/raw"
