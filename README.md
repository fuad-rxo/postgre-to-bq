# postgre-to-bq
postgre-to-bq-test

<img width="725" height="525" alt="2026-02-02_15-52" src="https://github.com/user-attachments/assets/36b1d7e1-62c4-4e34-84fa-7ae2dff87c5b" />

# 1. PostgreSQL
Direct Transfer:
Use psycopg2 to connect and fetch data
Load into pandas DataFrame
Push directly to BigQuery using bq load or API
Best for: Small-to-medium datasets, simple ETLs
Staging via GCS:
Export to CSV/Parquet locally
Upload to GCS
Load into BigQuery from GCS
Best for: Large datasets, incremental loads, or when network stability is a concern
