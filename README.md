# Football Stadiums Data Engineer

This python-based project crawls data from https://en.wikipedia.org/wiki/List_of_association_football_stadiums_by_capacity using Azure Databricks, cleans it and pushes it Azure Data Lake for processing. Later on we will be visualising the data via Power BI to gain business insights.

## Table of contents

1. [System Architecture](#system-architecture)
2. [Requirements](#requirements)
3. [Web Crawling](#web-crawling)
6. [Azure](#azure)
7. [Power BI](#power-bi)
8. [Video](#video)

## System Architecture
![system_architecture](https://github.com/user-attachments/assets/7afa1916-d20e-4151-9be5-95840d77fa98)

## Requirements
**Accounts:**
  - Databricks
  - Power BI
  - Microsoft

**Technologies:**
  - Azure Datalake Storage Gen 2
  - Azure Databricks
  - Python 3.12
  - Pip
  - Power BI
  - Azure HDInsight
  - Azure Data Factory

## Web Crawling
1. We open a terminal inside Databricks. We execute this commands: 
```bash
touch requirements.txt
nano requirements.txt
```
2. Inside requirements.txt we add the contents in the file: Requirements/requirements.txt
```bash
pip install -r requirements.txt
```
This will copy install all the libraries and dependencies inside requirements.txt
NOTE: there are more libraries and dependencies than the ones you need.

3. When executing the notebook, it will excract and clean all the data from the stadiums from wikipedia, later on saving them into a Dataframe.

4. Finally, the dataframe is saved as a csv inside a container in a datalake. You must change de SSA Key and the name of the container to the ones in your Datalake storage.



