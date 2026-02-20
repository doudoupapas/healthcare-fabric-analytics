# Healthcare Operations Analytics — Microsoft Fabric

## Overview
End-to-end data engineering project built on Microsoft Fabric demonstrating 
medallion architecture, multi-source ingestion, and automated CI/CD deployment.

## Architecture
- **Bronze**: Raw ingestion from CDC REST API, Azure SQL Database, Excel
- **Silver**: Cleaned, typed and enriched datasets
- **Gold**: Business-ready aggregates for Power BI

## Tech Stack
- Microsoft Fabric (Lakehouse, Notebooks, Pipelines, Power BI)
- Azure SQL Database
- Microsoft Entra ID (OAuth2 authentication — no credentials stored in Fabric)
- GitHub (source control)
- Azure DevOps (CI/CD)

## Security
Authentication to Azure SQL Database is handled through **Microsoft Entra ID (OAuth2)**
— no credentials or passwords are stored anywhere in Fabric or the repository.
Fabric connects to Azure SQL using an Organizational account, with access governed
by Entra ID roles and policies.

## How to Run
1. Clone this repository
2. Configure Azure credentials in pipeline variables
3. Push to main branch to trigger deployment
