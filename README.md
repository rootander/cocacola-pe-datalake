# 🥤 Coca-Cola Perú

# Azure Data Lake Storage Gen2 Architecture

<div align="center">

### Enterprise Cloud Data Platform Simulation

Azure Data Lake Storage Gen2 • Data Governance • Metadata Management • Cloud Architecture

![Azure](https://img.shields.io/badge/Azure-Data%20Lake%20Gen2-0078D4?style=for-the-badge\&logo=microsoftazure)
![Architecture](https://img.shields.io/badge/Architecture-Medallion-blue?style=for-the-badge)
![Storage](https://img.shields.io/badge/Storage-Hierarchical%20Namespace-green?style=for-the-badge)
![Governance](https://img.shields.io/badge/Data-Governance-orange?style=for-the-badge)

</div>

---

# 📖 Project Overview

This project simulates an **Enterprise Azure Data Lake Storage Gen2 Architecture** inspired by modern cloud data platforms used by multinational organizations such as Coca-Cola.

The architecture is designed following **Lakehouse and Medallion Architecture principles**, allowing data to be organized, governed, and stored efficiently across multiple layers while maintaining scalability, traceability, and data quality.

The solution demonstrates how enterprise data can be managed from its initial ingestion through trusted business-ready datasets while supporting governance, metadata management, and historical retention.

---

# 🏛️ Architecture Used

## Medallion Architecture

The Data Lake follows the **Medallion Architecture Pattern**, a modern data engineering approach widely adopted in cloud platforms.

```text
Landing
   │
   ▼
Bronze
   │
   ▼
Silver
   │
   ▼
Trusted
   │
   ▼
Archive
```

### Benefits

✅ Scalability

✅ Data Governance

✅ Data Quality Management

✅ Auditability

✅ Historical Preservation

✅ Enterprise Data Management

---

# ☁️ Technology Stack

| Component         | Technology                     |
| ----------------- | ------------------------------ |
| Cloud Platform    | Microsoft Azure                |
| Storage           | Azure Data Lake Storage Gen2   |
| Namespace         | Hierarchical Namespace (HNS)   |
| Data Organization | Medallion Architecture         |
| Governance        | Metadata Layer                 |
| Data Types        | Structured & Unstructured Data |
| Storage Model     | Data Lake                      |

---

# 🏗️ Data Lake Architecture

```text
                              ┌─────────────────────┐
                              │ Source Systems      │
                              │ OLTP • APIs • Files │
                              └──────────┬──────────┘
                                         │
                                         ▼
                          ┌─────────────────────────┐
                          │       LANDING           │
                          │ Raw Source Data         │
                          └──────────┬──────────────┘
                                     │
                                     ▼
                          ┌─────────────────────────┐
                          │        BRONZE           │
                          │ Domain Data Storage     │
                          └──────────┬──────────────┘
                                     │
                                     ▼
                          ┌─────────────────────────┐
                          │         SILVER          │
                          │ Standardized Datasets   │
                          └──────────┬──────────────┘
                                     │
                                     ▼
                          ┌─────────────────────────┐
                          │        TRUSTED          │
                          │ Business Ready Data     │
                          └──────────┬──────────────┘
                                     │
                                     ▼
                          ┌─────────────────────────┐
                          │        ARCHIVE          │
                          │ Historical Retention    │
                          └─────────────────────────┘


             ┌────────────────────────────────────────────┐
             │               METADATA LAYER               │
             │ Lineage • Governance • Schemas • Catalog   │
             └────────────────────────────────────────────┘
```

---

# 🔵 Landing Layer

The Landing Layer stores data exactly as received from source systems.

## Purpose

* Preserve original source data
* Maintain complete traceability
* Enable data lineage
* Support future reprocessing

## Data Sources

* OLTP Databases
* APIs
* CSV Files
* Excel Files
* JSON Files
* External Data Sources

```text
landing/
├── oltp_cocacola_ventas/
├── oltp_cocacola_clientes/
├── oltp_cocacola_productos/
└── external_sources/
```

---

# 🟤 Bronze Layer

The Bronze Layer organizes raw business data by enterprise domains.

## Business Domains

* Sales
* Customers
* Products
* Inventory
* Logistics
* Finance
* Production
* Marketing
* Human Resources

```text
bronze/
├── sales/
├── customers/
├── products/
├── inventory/
├── logistics/
├── finance/
├── production/
├── marketing/
└── hr/
```

---

# ⚪ Silver Layer

The Silver Layer contains standardized datasets with consistent structures.

## Characteristics

* Standardized formats
* Consistent schemas
* Data organization
* Improved usability

```text
silver/
├── sales/
├── customers/
├── products/
├── inventory/
├── logistics/
├── finance/
├── production/
└── marketing/
```

---

# 🟢 Trusted Layer

The Trusted Layer stores validated and business-ready information.

## Benefits

* Reliable datasets
* High-quality information
* Business consumption
* Governance compliance

```text
trusted/
├── sales/
├── customers/
├── products/
├── inventory/
├── logistics/
├── finance/
└── production/
```

---

# ⚫ Archive Layer

Long-term historical storage used for compliance and auditing.

## Benefits

* Historical preservation
* Regulatory compliance
* Audit support
* Disaster recovery

```text
archive/
```

---

# 🧠 Metadata Layer

Provides governance and management capabilities across the Data Lake.

## Includes

* Data Lineage
* Data Catalog
* Dataset Descriptions
* Schema Definitions
* Source Systems
* Ingestion Timestamps
* Ownership Information

```text
metadata/
```

---

# 📦 Unstructured Data Zone

Stores non-relational enterprise information.

## Examples

* Images
* Videos
* PDFs
* Documents
* Logs
* Multimedia Files

```text
unstructured/
```

---

# 📂 Repository Structure

```text
datalake/
│
├── landing/
│   ├── oltp_cocacola_ventas/
│   ├── oltp_cocacola_clientes/
│   ├── oltp_cocacola_productos/
│   └── external_sources/
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
│
├── trusted/
│
├── metadata/
│
├── unstructured/
│
└── archive/
```

---

# 🎯 Project Objective

Design and document an enterprise-scale Azure Data Lake Storage Gen2 architecture demonstrating:

* Data Lake best practices
* Cloud-native storage design
* Data governance principles
* Metadata management
* Domain-driven organization
* Enterprise data lifecycle management

---

# 🚀 Key Features

✔ Azure Data Lake Storage Gen2

✔ Hierarchical Namespace (HNS)

✔ Medallion Architecture

✔ Metadata Management

✔ Data Governance

✔ Structured Data Storage

✔ Unstructured Data Storage

✔ Historical Data Retention

✔ Enterprise Domain Organization

✔ Scalable Cloud Architecture

---


# 👨‍💻 Authors

- Lucas Cocha — Cloud Engineer
- Quispe Sebastian — Data Analyst

Enterprise Data Engineering Project

Azure Data Lake Storage Gen2 Architecture
