# Project-Optum-DBx

# Optum - Healthcare Data Engineering Project

## Overview

Optum is a healthcare data engineering solution built on Azure Cloud using Medallion Architecture. The platform processes healthcare insurance, subscriber, claims, patient, hospital, and disease datasets to provide analytics-ready data for business reporting and healthcare insights.

---

## Architecture

Source Systems
        |
        v
Azure Blob Storage
        |
        v
Azure Data Factory
        |
        v
ADLS Gen2 (Bronze Layer)
        |
        v
Azure Databricks
        |
        v
Silver Layer
        |
        v
Gold Layer
        |
        v
Power BI / Reporting

---

## Technologies Used

- Azure Blob Storage
- Azure Data Lake Storage Gen2
- Azure Data Factory
- Azure Databricks
- Azure Key Vault
- GitHub
- PySpark
- Azure SQL Database

---

## Data Domains

### Group

Contains insurance provider information.

### Sub Group

Insurance plans under each provider.

### Subscriber

Policy holder information.

### Claims

Insurance claim transactions.

### Patient

Patient healthcare details.

### Hospital

Hospital master records.

### Disease

Disease reference dataset.

---

## Medallion Architecture

### Bronze Layer

- Raw Data Ingestion
- Source Preservation
- Audit Tracking

### Silver Layer

- Data Cleansing
- Validation
- Standardization
- Deduplication

### Gold Layer

- Business Transformations
- Fact and Dimension Tables
- Analytics Datasets

---

## Security

Azure Key Vault is used for:

- Secrets Management
- Service Principal Credentials
- Storage Access Keys
- Pipeline Authentication

---

## Analytics Use Cases

- Claims Analysis
- Disease Trend Analysis
- Hospital Performance Analysis
- Subscriber Insights
- Insurance Reporting

---

## Repository Structure

```text
Optum/
│
├── Notebooks
├── Medallion/
│   ├── bronze/
│   ├── silver/
│   └── gold/
│
├── pipelines/
│   ├── adf/
│
├── configs/
│
├── datasets/
│
├── docs/
│
└── README.md
```

---

## Author

Healthcare Data Engineering Project using Azure Data Platform and Databricks.
