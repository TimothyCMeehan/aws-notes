# AWS Organizations
- Global Service
- Allows to manage multiple AWS accounts
- The main account is the master account
- Cost benefits:
    - Consolidated Billing across all accounts - single payment method
    - Pricing benefits from aggregated usage (volume discount for EC2, S3...)
    - Pooling of reserved EC2 instances for optimal savings
- API is available to automate AWS account creation
- Restrict account privileges using Service Control Policies (SCP)
## Multi Account Strategies
- Create accounts per department, per cost center, per dev / test/ prod, based on regulatory restrictions (using SCP), for better resource isolation (ex:VPC), to have separate per-account service limits, isolated account logging
- Multi Account vs One Account Multi VPC
- Use tagging standards for billing purposes
- Enable Cloud Trail on all accounts, send logs to central S3 account
- Send CloudWatch Logs to central logging account
## Service Control Policies (SCP)
- Whitelist or blacklist IAM actions
- Applied at the OU or Account level
- Does not apply to the Master Account
- SCP is applied to all the Users and Roles of the Account, including Root
- The SCP does not affect service-linked roles
    - Service-linked roles enable other AWS services to integrate with AWS Organizations and can't be restricted by SCPs.
- SCP must have an explicit Allow (does not allow anything by default)
- Use cases:
    - Restrict access to certain services
    - Enforce PCI compliance by explicitly disabling services