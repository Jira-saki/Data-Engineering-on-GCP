
# GCP ETL Pipeline using Cloudcomposer, Apache Airflow, Cloud Storage. 
![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/GCP_ETL.png)

# Introduction & Goals
- Introduce your project to the reader
- Orient this section on the Table of contents
- Write this like an executive summary
  - With what data are you working
  - What tools are you using
  - What are you doing with these tools
  - Once you are finished add the conclusion here as well

# Contents

- [The Data Set](#the-data-set)
- [Used Tools](#used-tools)
  - [Connect](#connect)
  - [Processing](#processing)
  - [Storage](#storage)
- [Pipelines](#pipelines)
  - [Batch Processing](#batch-processing)
  - [Visualizations](#visualizations)
- [Conclusion](#conclusion)
- [Follow Me On](#follow-me-on)
- [Appendix](#appendix)


# The Data Set
- The dataset of online audible purchase is from MySQL Database and REST API ingested. 


# Used Tools
- Python, CLI , Cloudcomposer, Apache Airflow, Google cloud Storage,Big query.


## Connect
## Buffer
# Processing
- Setting environment in cloud composer and use DAG in Airflow for orchastration.

- ![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/create-pipeline.png)
- ![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/set-env-01.png)
- ![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/set-env-02.png)

- Install PyPI choosing PySQL, requests, Pandas
- ![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/install_PyPI.png)

- Bucket of Airflow will be created in Cloud storage
- ![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/bucket-from-airflow.png) 

- Load Dags Python file to bucket at DAGS folder 
-  ![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/load-dags-to-gcs.png)

- Connect Airflow with MySQL
- ![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/connect-mysql.png)

- Run Dags
- ![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/final_dags.png)

- Output ETL Data will be loaded to Cloud coposer Bucket ready to tranfer to BigQuery for analysis. 
![alt text](https://github.com/Jira-saki/ETL-Pipeline-GCP/blob/main/image/output-bucket.png)


## Storage
## Visualization

# Pipelines
- Cleaned data has been ingested in Data Lake bucket(Cloud storage).

## Stream Processing
### Storing Data Stream
### Processing Data Stream
## Batch Processing
## Visualizations



# Conclusion
Write a comprehensive conclusion.
- How did this project turn out
- What major things have you learned
- What were the biggest challenges

# Follow Me On
Add the link to your LinkedIn Profile

# Appendix

[Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
