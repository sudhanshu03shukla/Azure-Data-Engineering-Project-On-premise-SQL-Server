# Azure-Data-Engineering-Project-On-premise-SQL-Server

## **Introduction:**
This project demonstrates an end-to-end data engineering solution using an on-premises SQL Server as the source system and Azure cloud services. 
Data is ingested using Azure Data Factory and stored in ADLS Gen2 following the Medallion architecture (Bronze, Silver, Gold).
Databricks is used for scalable data transformation, with Azure Synapse enabling analytical querying and Power BI delivering business insights.

## **Dataset:**
We have used AdventureWorks database as SQL data source. 
The AdventureWorks database is a popular and widely-used sample database provided by Microsoft for SQL Server.

Go to : Microsoft GitHub repository:

  
    https://github.com/Microsoft/sql-server-samples/releases/tag/adventureworks

download the below db backup:\
AdventureWorks2022.bak \

Go on this link to learn how to restore the db in SSMS :

    https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver16&tabs=ssms
