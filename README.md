
# ETL Pipeline on Google Cloud Platform. 

![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/GCP_ETL.png)

# Introduction & Goals
- This ETL Pipeline project is a part of [R2DE](https://school.datath.com/courses/road-to-data-engineer-2/dashboard) Data engineering course.
- ETL job of transaction audible data and audible book ID, extract to Apache Airflow , Transform data, loading to Data lake destination.
- Load specific data table to BigQuery for further analysis and visualisation. 


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
- Python, CLI , Cloud Composer (Apache Airflow), Cloud Storage, BigQuery, Data Studio.



# Processing

- Setting environment in cloud composer.

![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/set-env-01.png)
![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/set-env-02.png)






- Install PyPI choosing Pymysql, requests, Pandas


![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/install_PyPI.png)


- New bucket of Airflow has created in Cloud Storage

![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/bucket-from-airflow.png) 



- Load [Dags](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/dag_code) Python code to bucket at DAGS folder 

![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/load-dags-to-gcs.png)




- Connect Airflow with MySQL

- Run Dags

![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/final_dags.png)



- Output ETL Data will be loaded to Cloud Storage Bucket. 


![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/output-bucket.png)



- Manually load dataset to BigQuery. Create dataset and table for further query or BI tool. 


![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/load-table-from-bucket.png)


- Visualisation of data in Google Data Studio 


![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/dashboard.png)


# Pipelines
- DAGS
  Task 1:Get data from MySQL
  Task 2:Get data from API and change conversion rate.
  Task 3:Merge two data sets
- Load output data to Data Lake bucket(Cloud storage).
- Create dataset in data warehouse (BigQuery) and load table for query and visualisation.




# Follow Me On
https://www.linkedin.com/in/jirasak-pakdeeto-900665214/

# Appendix

[Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
