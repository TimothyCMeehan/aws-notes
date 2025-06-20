# Redshift Overview
- Redshift is based on PostgreSQL, but is not used for OLTP (Online Transaction processing)
- It's OLAP - online analytical processing (analytics and data warehousing)
- Load data once ever hour, not every second
- 10x better performance that other data warehouses, scales to PBs of data
- Columnar storage of data (instead of row based)
- Massively Parallel Query Execution (MPP), highly available
- Pay as you go based on instances provisioned
- Has a SQL interface for performing the queries
- BI tools such as AWS Quicksight or Tableau integrate with it
## Redshift Serverless
- Automatically provisions and scales data warehouse underlying capacity
- Run analytics workloads without managing data warehouse infrastructure
- Pay only for what you use (save costs)
- Use cases: Reporting, dashboarding applications, real-time analytics
