# Disaster Recovery Strategies
- Backup and Restore
    - Backup Data in S3
- Pilot Light
    - Core functions of the App Ready to scale, but minimum setup
- Warm Standby
    - full version of app, but minimum size
- Multi-Site / Hot-Site
    - full version of the app at full size
## AWS Elastic Disaster Recovery (DRS)
- Used to be named 'CloudEndure Disaster Recovery'
- Quickly and easily recover your physical, virtual, and cloud-based servers into AWS
- Example: protect your most critical databases (including Oracle, MySQL, and SQL Server), enterprise apps (SAP), protect your data from ransomware attacks, ...
- Continuos block-level replication for your servers