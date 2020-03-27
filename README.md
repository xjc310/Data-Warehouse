# Data Warehouse
## Introduction
The datasets are as follows:
●	CMS Medicare Part D Drug Spending
●	Medicare Provider Utilization and Payment Data: Part D Prescriber
Specifically, CMS Medicare Part D Drug Spending data comprises the data from 2013-2017; and Medicare Provider Utilization and Payment Data: 
Part D Prescriber comprises the data from 2013 to 2016. The datasets we chose are about prescription drugs prescribed by individual physicians 
and other health care providers and paid for under the Medicare Part D Prescription Drug Program. Medicare is the health insurance plan provided 
by the government for people above 65 years of age or for people with disabilities. We have chosen to use the data of Medicare Part D which deals 
with coverage related to prescription drugs. As a Business Intelligence project, the process is as follows: Data Integration -> Data Warehousing -> Business Intelligence. 

## Objectives
We have selected two datasets to work on our project they are the CMS Medicare Provider Utilization and Payment Data and CMS Medicare Part D Drug Spending Dashboard and Data. 
We identified the primary key  and foreign keys of the tables. After identification of the primary and foreign keys we will clean the source datasets to carry out further 
processes. We created a schema in which we created the dimensions and fact tables. Once the dimensions and facts have been created we populate these tables using ETL processes 
to create a data warehouse and build OLAP cubes. Our main objective to perform these steps is to get insight to make meaningful analysis and visualization to find the correlation 
between these two datasets.


## Dataset Description

CMS Medicare Provider Utilization and Payment Data
This dataset provides the data on drugs prescribed by health care providers and covered under the Medicare part D program. The healthcare care providers have been provided with 
a unique 10 digit identification number called the National Provider Identifier. Since the NPI has unique values we will use it as a primary key.Also we will use  Drug Name column 
as foreign key to refer to the other dataset “CMS Medicare Part D Drug Spending Data”. There are 21 columns in the dataset and around 25 million rows in each table from different 
years. The column names are as follows: npi, nppes_provider_last_org_name, nppes_provider_first_name, nppes_provider_city, nppes_provider_state, specialty_desc, description_flag, 
drug_name, generic_name, bene_count, total_claim_count, total_30_day_fill_count, total_day_supply, total_drug_cost, bene_count_ge65, bene_count_ge65_redact_flag, total_claim_count_ge65, 
ge65_redact_flag, total_30_day_fill_count_ge65, total_day_supply_ge65, and total_drug_cost_ge65.


CMS Medicare Part D Drug Spending Dashboard & Data
This dataset presents spending information for Medicare Part D drugs - drugs patients generally administer themselves and that are paid through the Medicare Part D program. Part D drug 
information is available from the Part D Prescription Drug Event (PDE) data, which are available for a subset of Medicare beneficiaries who choose to enroll in Part D (which represents 
approximately 70% of Medicare beneficiaries). The dataset is about Medicare Part D Drug Spending and Utilization from Calendar Years 2013 to 2017. There are 13 columns in the dataset, 
they are showing as follows: Brand Name, Generic Name, Manufacturer, Number of Manufacturers, Total Spending, Total Dosage Units, Total Claims, Total Beneficiaries, Average Spending 
Per Dosage Unit (Weighted), Average Spending Per Claim, Average Spending Per Beneficiary, Change in Average Spending Per Dosage Unit (2016-2017), and Annual Growth Rate in Average 
Spending Per Dosage Unit (2013-2017). The brand name is the primary key.
