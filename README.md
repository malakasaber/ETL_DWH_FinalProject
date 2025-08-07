# ETL & Data Warehouse Final Project

## Overview

Designed and implemented a Data Warehouse using a star schema featuring transactional fact tables with fully additive measures. Automated the ETL pipeline—including incremental loading, transformations, and loading into the DWH—using SSIS. Deployed, queried, and scheduled data workflows via SSMS. Built an interactive Power BI dashboard to visualize insights from the data warehouse.

---

## Project Structure

```
ETL_DWH_FinalProject/
│
├── ETL/                   # SSIS packages for extraction, transformation, incremental loading
│
├── DWH/                   # Star schema definitions and database setup scripts
│   ├── dimension_tables.sql
│   └── fact_tables.sql
│
├── SSMS/                  # SSMS jobs and deployment configurations
│   ├── schedule_jobs.sql
│   └── deployment_notes.md
│
├── Dashboard/             # Power BI dashboard files and templates
│   └── shipping_dashboard.pbix
│
└── README.md              # Project documentation (this file)
```

---

## Features & Workflow

1. **Data Warehouse & Schema Design**

   * Modeled a star schema with fact and dimension tables for efficient querying and analytics.

2. **ETL Automation with SSIS**

   * Built SSIS packages to handle incremental extraction, data transformations, and loading into the DWH.

3. **Workflow Scheduling via SSMS**

   * Automated workflows using SQL Server Agent for deployment, execution, and scheduling of ETL processes.

4. **Business Intelligence (Power BI Dashboard)**

   * Created an interactive Power BI dashboard to visualize KPIs and insights extracted from the data warehouse.

---

## Setup & Usage

### Step 1: Configure the Warehouse

* Run SQL scripts under `DWH/` in your SQL Server environment to create the star schema.

### Step 2: Load ETL Packages

* Open the `.dtsx` files in the `ETL/` directory using Visual Studio or SSDT.
* Adjust data source settings and deploy packages to your SSIS catalog.

### Step 3: Schedule Jobs

* Import job scripts from `SSMS/` into SQL Server Agent.
* Review and customize scheduling based on your requirements.

### Step 4: Access Dashboard

* Open the Power BI `.pbix` file from the `Dashboard/` folder.
* Refresh data sources to connect with your configured DWH and explore insights.

---

## Technologies & Tools

| Component        | Tools Used                                                                  |
| ---------------- | --------------------------------------------------------------------------- |
| ETL & Automation | SQL Server Integration Services (SSIS), SQL Server Management Studio (SSMS) |
| Data Modeling    | Star Schema Design, Transactional Fact Tables                               |
| Visualization    | Power BI                                                                    |

---

## Contribution

Feel free to adapt schema elements, modify SSIS logic, or enhance visualizations. Pull requests and improvements are welcome!

---

## License

This project is available under the MIT License. Feel free to reuse and modify components!
