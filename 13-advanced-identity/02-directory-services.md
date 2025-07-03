# AWS Directory Services
## What is Microsoft Active Directory (AD)?
- Found on any Windows Server with AD Domain Services
- Database of objects: User Accounts, Computers, Printers, File Shares, Security Groups
- Centralized security management, create account, assign permissions
## Directory Services
- AWS Managed Microsoft AD
    - Create your own AD in AWS, manage users locally, supports MFA
    - Establish 'trust' connections with your on-premise AD
- AD Connector
    - Directory Gateway (proxy) to redirect to on-prem AD, supports MFA
    - Users are managed on the on-prem AD
- Simple AD
    - AD-compatible managed directory on AWS
    - Cannot be joined with on-premise AD