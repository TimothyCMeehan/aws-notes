# AWS STS (Security Token Service)
- Enables you to create temporary, limited-privleges credentials to access your AWS resources
- Short-term credentials: you configure expiration period
- Use cases:
    - Identity federation: manage user identities in extrenal systems, provide them with STS tokens to access AWS resources
    - IAM Roles for cross/same account access
    - IAM Roles for EC2: provide temporary credentials for EC2 instances to access AWS resources