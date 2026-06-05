<p align="center">
  <img src="images/architecture.png" width="1000">
</p>

<h1 align="center">🥤 Coca-Cola Perú</h1>

<h3 align="center">Azure Data Lake Storage Gen2 Architecture</h3>

<p align="center">
Enterprise Data Engineering Project
</p>

<p align="center">
Azure Data Lake • Cloud Storage • Data Governance • Metadata Management
</p>

---

## 📖 Overview

This project simulates an enterprise-grade **Azure Data Lake Storage Gen2** architecture inspired by modern cloud data platforms used by large organizations such as Coca-Cola.

The repository focuses on the organization, storage, and governance of enterprise data following Data Lake best practices and cloud-native architecture principles.

---

## ☁️ Technology Stack

* Microsoft Azure
* Azure Data Lake Storage Gen2
* Hierarchical Namespace
* Structured Data Storage
* Unstructured Data Storage
* Metadata Management

---

## 🏗️ Data Lake Architecture

### Data Flow

```text
Landing → Bronze → Silver → Trusted → Archive
```

<p align="center">
  <img src="images/datalake-architecture.png" width="900">
</p>

---

## 🔵 Landing Layer

Initial ingestion area where data arrives directly from source systems in its original format.

**Purpose**

* Preserve original source data
* Maintain traceability
* Store incoming files without modification

---

## 🟤 Bronze Layer

Raw data storage organized by business domains.

**Domains**

* Sales
* Customers
* Products
* Inventory
* Logistics
* Finance
* Production
* Marketing
* Human Resources

<p align="center">
  <img src="images/bronze-layer.png" width="800">
</p>

---

## ⚪ Silver Layer

Standardized and organized datasets with consistent structures and formats.

**Characteristics**

* Structured datasets
* Standardized schemas
* Improved consistency
* Organized business information

<p align="center">
  <img src="images/silver-layer.png" width="800">
</p>

---

## 🟢 Trusted Layer

Validated and trusted datasets representing the official version of business information.

**Benefits**

* Reliable datasets
* Data consistency
* Enterprise-ready information
* Governance compliance

<p align="center">
  <img src="images/trusted-layer.png" width="800">
</p>

---

## ⚫ Archive Layer

Long-term storage area used for historical retention, auditing, and compliance requirements.

**Benefits**

* Historical preservation
* Regulatory compliance
* Audit support
* Data recovery

---

## 🧠 Metadata Layer

Provides governance and management information for all datasets stored in the Data Lake.

**Includes**

* Data Lineage
* Source Systems
* Dataset Descriptions
* Schema Definitions
* Ingestion Timestamps

<p align="center">
  <img src="images/metadata-layer.png" width="800">
</p>

---

## 📦 Unstructured Data

Storage area for non-relational content.

**Examples**

* Images
* PDFs
* Videos
* Documents
* Logs
* Multimedia Files

<p align="center">
  <img src="images/unstructured-data.png" width="800">
</p>

---

## 📂 Repository Structure

```text
datalake/
│
├── landing/
│   └── oltp_cocacola_ventas/
│
├── bronze/
│   ├── sales/
│   ├── customers/
│   ├── products/
│   ├── inventory/
│   ├── logistics/
│   ├── finance/
│   ├── production/
│   ├── marketing/
│   └── hr/
│
├── silver/
│   ├── sales/
│   ├── customers/
│   ├── products/
│   ├── inventory/
│   ├── logistics/
│   ├── finance/
│   ├── production/
│   └── marketing/
│
├── trusted/
│   ├── sales/
│   ├── customers/
│   ├── products/
│   ├── inventory/
│   ├── logistics/
│   ├── finance/
│   └── production/
│
├── metadata/
├── unstructured/
└── archive/
```

---

## 🎯 Project Objective

Design and document a scalable Azure Data Lake Storage Gen2 architecture demonstrating enterprise-level storage organization, governance, and cloud data management practices.

---

## ⚠️ Scope

This project represents only the Data Lake storage architecture and does not include:

* ETL / ELT Pipelines
* Azure Data Factory
* Azure Synapse Analytics
* Data Warehouse
* Data Marts
* Power BI Dashboards
* Machine Learning
* Advanced Analytics

---

## 👨‍💻 Author

**Lucas David**

Data Engineering Portfolio Project
