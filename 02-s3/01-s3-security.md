# Amazon S3 - Security
- User-Based
    - IAM Policies - which API calls should be allowed for a specific user from IAM
- Resource-Based
    - Bucket Policies - bucket wide rules from the S3 console - allows cross account
    - Object Access Control List (ACL) - finer grain (can be disabled)
    - Bucket Access COntrol List (ACL) - less common (can be disabled)
- Note: anIAM proncipam can access an S3 Object if
    - The user IAM permissions ALLOW it OR the resource policy ALLOWS it
    - AND there's no explicit DENY
- Encryption: encrypt objects in Amazon S3 using encyption keys
    - Server-Side Encryption (Default)
## S3 Bucket Policies
- JSON based policies
    - Resources: buckets and objects
    - Effect: Allow / Deny
    - Actions: Set of API to Allow or Deny
    - Principal: The account or user to apply the policy to
- Use S3 bucket for policy to:
    - Grant public access to the bucket
    - Force objects to be encypted at upload
    - Grant access to another account (Cross Account)
## Bucket settings for Block Public Access
- These settings created to prevent company data leaks
- If you know your bucket should never be public, leave these on
- Can be set at the account level
## IAM Access Analyzer for S3
- Ensures that only the intended people have access to your S3 buckets
- Evaluates S3 Bucket Policies, S3 ACLs, S3 Access Point Policies
