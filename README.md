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

## **Project Architecture:**
![project_architecture](screenshots/Project_architecure.png)

## **Create Azure Resources for the project:**

### **Create Resource Group:**
Create a resource group in Azure portal to hold all the other resources.

### **Create Azure Data Factory:**
Resource Group > Create > Azure Data Factory > Create > (give data factory name, resource group, subscription and create)

### **Create Azure Synapse Analytics and Storage Account:**
Resource Group > Create > Azure Synapse Analytics > Create > 
#### Basics Tab (Project Details) :
Choose your subscription and resource group (This will be automatically selected)\
Ignore the Managed resource group drop down. (This will be automatically created if not specified)

![synapse_storage](screenshots/synapse_storagegrp.png)

1. Account Name (This is the Storage Account Name)- Click on the "Create new" link and give it a name.
2. File System Name (This is the container name)- Click on the "Create new" link and give it a name as "bronze".
3. Review and create.

### **Create Azure Databricks:**
Resource Group > Create > Azure Data Factory > Create > (give data bricks resource name, resource group, subscription and create)

## **All Azure Resources for the project:**
![all_resource](screenshots/All_azure_resource.png)
