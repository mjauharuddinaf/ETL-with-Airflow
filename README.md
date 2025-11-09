# ETL-with-Airflow
ETL from Multiple Data Sources to GBQ with Airflow

In this project, I will perform ETL from several data sources using Airflow into Google BigQuery.
The steps are as follows:
1. Use data from bigquery-public-data.new_york_taxi_trips.
2. From several tables in that dataset, I create multiple files in different formats, such as JSON, CSV (on local device), Google Spreadsheet, CSV (uploaded to Google Drive), and CSV (uploaded to GitHub).
3. Then, I configure Airflow to perform the ETL process using the data from point 2 above.
4. In addition to performing ETL, I will also conduct Data Quality checks to ensure whether the ETL results are accurate, such as checking for NULL values, duplicate data based on ID granularity, and missing value mappings.
5. If there are data quality issues, I will load those records into the table ny_taxi_raw_unpublish.
6. For data that passes the quality checks, I will load it into the table ny_taxi_raw_publish.
7. From the ny_taxi_raw_publish table, I will create new tables containing aggregated data (daily and monthly)
