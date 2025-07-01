# VPC Endpoints
- Endpoints allow you to connect to AWS Services using private network instead of public www network
- This gives you enhanced security and lower latency to access AWS services
- VPC Endpoint Gateway: S3 & DynamoDB
- VPC Endpoint Interface: most services (including s3 and DynamoDB)
## AWS PrivateLink
- Most secure and scalable way to expose a service to 1000s of VPCs
- Does not require VPC peering, internet gateway, NAT, route tables...
- Requires a network load balancer (Service VPC) and ENI (Customer VPC)
## Site to Site VPN & Direct Connect
- Site to Site VPN
    - Connect an on-prem VPN to AWS
    - The connection is automatically encrypted
    - Goes over the public internet
    - On-prem: must use a Customer Gateway (CGW)
    - AWS: must use a Virtual Private Gateway (VGW)
- Direct Connect (DX)
    - Establish a physical connection between on-prem and AWS
    - The connection is private , secure and fast
    - Goes over a private network
    - Takes at least a month to establish
## AWS Client VPN
    - Connect from your computer using OpenVPN to your private network in AWS and on-prem
    - Allows you to connect to your EC2 instances over a preivate IP (just as if you were in the private VPC network)
    - Goes over public internet
## Transit Gateway
- For having a transitive peering beteen thousands of VPC and on-prem, hub and spoke (star) connection
- One single Gateway to provide this functionality
- Works with Direct Connect Gateway, VPN connections