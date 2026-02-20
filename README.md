# Healthcare Operations Analytics — Microsoft Fabric

# Overview
End-to-end data engineering project built on Microsoft Fabric demonstrating 
medallion architecture, multi-source ingestion, and automated CI/CD deployment.

# Architecture
- Bronze: Raw ingestion from CDC REST API, Azure SQL Database, Excel
- Silver: Cleaned, typed and enriched datasets
- Gold: Business-ready aggregates for Power BI

 # Tech Stack
- Microsoft Fabric (Lakehouse, Notebooks, Pipelines, Power BI)
- Azure SQL Database
- Azure Key Vault
- GitHub (source control)
- Azure DevOps (CI/CD)

 # CI/CD
Automated deployment pipeline triggers on every push to main branch,
validates notebooks and deploys to Fabric Dev workspace via REST API.

# How to Run
1. Clone this repository
2. Configure Azure credentials in pipeline variables
3. Push to main branch to trigger deployment
