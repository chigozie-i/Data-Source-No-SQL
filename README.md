![Connect to NoSQL](https://github.com/chigozie-i/Data-Source-No-SQL/blob/main/No%20SQL%20Hero.png)

## Introduction:
In today’s data driven world, organizations rely heavily on insights derived from data to drive strategic decision-making and enhance operational efficiency. Microsoft Power BI stands as a powerful tool in this landscape, offering robust capabilities for connecting to various data sources, transforming raw data into meaningful insights, and creating interactive visualizations and reports.

## Table of Contents

- [Overview](#Overview)
- [Data Sources](#Data-Sources)
- [Connecting To A NoSQL Database](#Connecting-To-A-NoSQL-Database)
- [Connecting To Azure Cosmos DB](#Connecting-To-Azure-Cosmos-DB)
- [Importing A JSON File](#Importing-A-JSON-File)
- [Conclusion](#Conclusion)
- [Reference](#Reference)
  
## Overview:

This document focuses on utilizing Microsoft Power BI for data analysis, forming part of a series of documentation projects aimed at exploring various methods for connecting to your data source. This document seeks to underscore the critical significance of selecting an appropriate data source connection method and to offer comprehensive guidance on the diverse approaches available for establishing connectivity to your data source prior to initiating any essential data transformations tailored to your analytical objectives.

The primary goal of this endeavor is to establish a dependable repository for your data, fostering operational efficiency and ensuring the accuracy of reporting in alignment with the business requirements.

The method by which you establish connectivity to your data source holds considerable importance, as it directly influences the efficiency of your analytical tools and shapes the user experience. Moreover, it plays a pivotal role in determining the effectiveness, precision, and trustworthiness of the analytical processes and resulting reports.


## Data Sources:
Sometimes, you may be required to build Microsoft Power BI reports, with data sourced from various databases and files. These data sources vary, with some housed in Microsoft SQL Server and others in Microsoft Excel, yet they are all interconnected.

![Data Sources](https://github.com/chigozie-i/Data-Source-No-SQL/blob/main/Data%20sources.png)

Prior to report creation, it's essential to extract data from the various data sources. As the interaction with the sources differ, familiarizing yourself with the intricacies of the source platforms is imperative to report building within Power BI.

#### Data Sources:

1.	Files
2.	Relational Data Sources | Create Dynamic Reports with Parameters
3.	NoSQL Database 
4.	Online Services
5.	Azure Analysis Services


This documentation project focuses on No SQL Database.

## Connecting To A NoSQL Database:
Certain organizations opt not to utilize relational databases and instead employ NoSQL databases. NoSQL databases, being versatile, do not rely on tables for data storage.  
  
In this case, Imaginary Inc. has developed an application aimed at overseeing the shipping and tracking of products from their warehouses. The application utilizes Cosmos DB, a NoSQL database, as its data repository. Data is organized into JSON documents, which are widely recognized file formats primarily employed for transmitting data between servers and web applications. Your task involves importing this data into a Power BI semantic model for reporting purposes.

## How To Connect To a NoSQL Database (Azure Cosmos DB)

To establish a connection to your data source, utilize the "Get data" function within Power BI Desktop. Then, opt for the "More..." option to find and establish a connection with the specific type of database you're using. In this instance, you'll navigate to the Azure category, choose Azure Cosmos DB, and proceed by selecting "Connect."

![Get Data](https://github.com/chigozie-i/Data-Source-No-SQL/blob/main/Connecting%20to%20NoSQL.png)

On the Preview Connector window, select Continue and then enter your database credentials. In this example, on the Azure Cosmos DB window, you can enter the database details. You can specify the Azure Cosmos DB account endpoint URL that you want to get the data from (you can get the URL from the Keys blade of your Azure portal). Alternatively, you can enter the database name, collection name or use the navigator to select the database and collection to identify the data source.
If you're connecting to an endpoint for the first time, make sure that you enter your account key. You can find this key in the Primary Key box in the Read-only Keys blade of your Azure portal.

## Importing a JSON File

When dealing with data stored in JSON format, it's frequently essential to extract and normalize the data beforehand. This is due to the tendency for JSON data to be stored in a nested or unstructured format, making direct analysis or reporting challenging. Consequently, you must transform the data prior to loading it into Power BI Desktop.  
  
Once you've established a connection to the database account, the Navigator window will appear, presenting a list of databases within that account. From this list, you'll choose the table you wish to import. In this illustration, the Product table will be selected. Notably, the preview pane exclusively displays Record items, as all records in the document are represented as a Record type in Power BI.

![JSON I](https://github.com/chigozie-i/Data-Source-No-SQL/blob/main/Importing%20JSON%20I.png)

Select the Edit button to open the records in Power Query.  
  
In Power Query, select the Expander button to the right side of the Column1 header, which displays the context menu with a list of fields. Select the fields that you want to load into Power BI Desktop, clear the Use original column name as prefix checkbox, and then select OK.

![JSON II](https://github.com/chigozie-i/Data-Source-No-SQL/blob/main/Importing%20JSON%20II.png)

Review the selected data to ensure that you're satisfied with it, then select Close & Apply to load the data into Power BI Desktop.

![JSON III](https://github.com/chigozie-i/Data-Source-No-SQL/blob/main/Importing%20JSON%20III.png)

The data has now been structured into a table format consisting of rows and columns. This enables data from Cosmos DB to be connected with data from other sources and eventually utilized in a Power BI report.

## Conclusion:

In this documentation project, we have explored the process of connecting to a NoSQL database, specifically Azure Cosmos DB, using Microsoft Power BI. NoSQL databases, known for their flexibility and ability to handle unstructured data, offer unique challenges and opportunities for data analysis and reporting.

By leveraging the capabilities of Power BI, organizations can extract, transform, and visualize data from NoSQL databases like Cosmos DB, enabling them to derive actionable insights and make informed decisions. The process begins with establishing a connection to the database, wherein users can specify database details such as the account endpoint URL and credentials.

Once connected, Power BI facilitates the transformation of JSON data into a structured format suitable for analysis and reporting. This involves extracting and normalizing the data to create a table with rows and columns. Through this process, data from Cosmos DB can be seamlessly integrated with other data sources, enhancing the depth and breadth of insights available for reporting purposes.

Ultimately, the ability to connect to NoSQL databases like Cosmos DB empowers organizations to harness the full potential of their data, driving innovation and competitive advantage in today's data-driven landscape. With Power BI as a powerful ally, organizations can unlock valuable insights from their NoSQL data, enabling them to stay ahead in an increasingly competitive market.

## Reference:
https://learn.microsoft.com  
https://docs.microsoft.com


## Help and Support

#### Did you find this document helpful? Leave a Star

[![GitHub stars](https://img.shields.io/github/stars/chigozie-i/Data-Source-No-SQL.svg?style=social)](https://github.com/chigozie-i/Data-Source-No-SQL/stargazers)

#### You may make a contribution to help us improve on our documentation by submitting a pull request.
