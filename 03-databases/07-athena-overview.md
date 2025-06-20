# Amazon Athena
- Serverless query service to perform analytics against S3 objects
- Uses standard SQL language to query files
- Supports CSV, JSON, ORC, Avro, and Parguet (built on Presto)
- Pricing: $5.00 per TB of data scanned
- Use compressed or columnar data for cost-savings (less scan)
- Use cases: Business intelligence / analytics / reporting, analyze & query VPC Flow Logs, ELB Logs, CloudTrail trails, etc...
- Exam Tip: analyze data in S3 using serverless SQL, use Athena