![Connect to NoSQL](https://github.com/chigozie-i/Data-Source-No-SQL/blob/main/No%20SQL%20Hero.png)

## Introduction:
In today’s data driven world, organizations rely heavily on insights derived from data to drive strategic decision-making and enhance operational efficiency. Microsoft Power BI stands as a powerful tool in this landscape, offering robust capabilities for connecting to various data sources, transforming raw data into meaningful insights, and creating interactive visualizations and reports.

## Table of Contents

- [Overview](#Overview)
- [Data Sources](#Data-Sources)
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

## Connecting To NoSQL:
Certain organizations opt not to utilize relational databases and instead employ NoSQL databases. NoSQL databases, being versatile, do not rely on tables for data storage.  
  
In this case, Imaginary Inc. has developed an application aimed at overseeing the shipping and tracking of products from their warehouses. The application utilizes Cosmos DB, a NoSQL database, as its data repository. Data is organized into JSON documents, which are widely recognized file formats primarily employed for transmitting data between servers and web applications. Your task involves importing this data into a Power BI semantic model for reporting purposes.

## Connecting To a NoSQL Database (Azure Cosmos DB)

To establish a connection to your data source, utilize the "Get data" function within Power BI Desktop. Then, opt for the "More..." option to find and establish a connection with the specific type of database you're using. In this instance, you'll navigate to the Azure category, choose Azure Cosmos DB, and proceed by selecting "Connect."

![]()

## Help and Support

#### Did you find this document helpful? Leave a Star

[![GitHub stars](https://img.shields.io/github/stars/chigozie-i/Data-Source-No-SQL.svg?style=social)](https://github.com/chigozie-i/Data-Source-No-SQL/stargazers)

#### You may make a contribution to help us improve on our documentation by submitting a pull request.
