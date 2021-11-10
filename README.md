
# GCP ETL Pipeline using Cloud Composer, Apache Airflow, Cloud Storage. 
![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/GCP_ETL.png)

# Introduction & Goals
- This project is about ETL job of transaction audible data and audible book ID, extract to Apache Airflow , Transform data, loading to Data lake destination. 


# Contents

- [The Data Set](#the-data-set)
- [Used Tools](#used-tools)
  - [Processing](#processing)
- [Pipelines](#pipelines)
- [Follow Me On](#follow-me-on)
- [Appendix](#appendix)


# The Data Set
- The dataset of online audible purchase is from MySQL Database and REST API ingested. 


# Used Tools
- Python, CLI , Cloud Composer, Apache Airflow, Google Cloud Storage.



# Processing

- Setting environment in cloud composer.

![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/set-env-01.png)
![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/set-env-02.png)
![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/create-pipeline.png)



- Install PyPI choosing Pymysql, requests, Pandas


![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/install_PyPI.png)


- New bucket of Airflow has created in Cloud Storage

![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/bucket-from-airflow.png) 

- Load Dags Python file to bucket at DAGS folder 

![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/load-dags-to-gcs.png)

- Connect Airflow with MySQL

![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/connect-mysql.png)

- Run Dags

![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/final_dags.png)


- Output ETL Data will be loaded to Cloud Storage Bucket. Copy data to BigQuery for analysis. 


![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/output-bucket.png)


# Pipelines
- DAGS
  Task 1:Get data from MySQL
  Task 2:Get data from API and change conversion rate.
  Task 3:Merge two data sets
- Load output data to Data Lake bucket(Cloud storage).




# Follow Me On
https://www.linkedin.com/in/jirasak-pakdeeto-900665214/

# Appendix

[Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
