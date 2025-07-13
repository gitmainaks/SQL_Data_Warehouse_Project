**Data Architecture**

The data architecture for this project follows Medallion Architecture **Bronze**, **Silver** and **Gold** layers: 

Sources ![](Aspose.Words.42b7b282-dfb4-4229-8548-b00b22dad631.001.png) Data Warehouse Consume![](Aspose.Words.42b7b282-dfb4-4229-8548-b00b22dad631.002.png)

Bronze Layer Silver Layer Gold Layer

Stored Procedure Stored Procedure

CRM BI & Reporting![](Aspose.Words.42b7b282-dfb4-4229-8548-b00b22dad631.003.png)![ref1]![ref2]![ref1]![ref2]

ERP

**Object Type:** CSV Files **Interface:** Files in Folder 

Raw Data

**Object Type:** Tables **Load:**

Batch Processing Full Load Truncate & Insert 

**No Tranformations Data Model:** None (as-is)

Cleaned,\
Standardized Data

**Object Type:** Tables **Load:**

Batch Processing Full Load Truncate & Insert 

**Tranformations:** 

Data Cleansing Data Standardization Data Normalization Derived Columns Data Enrichment 

**Data Model:** None (as-is)

Business Ready Data

**Object Type:** Views **No Load** **Tranformations:** 

Data Integrations Aggregations Business Logics

**Data Model:**

Star Schema Flat Table Aggregated Table

![](Aspose.Words.42b7b282-dfb4-4229-8548-b00b22dad631.006.png)

Ad-Hoc SQL Queries

![](Aspose.Words.42b7b282-dfb4-4229-8548-b00b22dad631.007.png)

Machine Learning 

[ref1]: Aspose.Words.42b7b282-dfb4-4229-8548-b00b22dad631.004.png
[ref2]: Aspose.Words.42b7b282-dfb4-4229-8548-b00b22dad631.005.png
