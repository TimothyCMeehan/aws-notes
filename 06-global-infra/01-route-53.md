# Amazon Route 53 Overview
- Route53 is a managed DNS (Domain Name System)
- DNS is a collection of rules and records which help clients understand how to reach a server through URLs
## Route 53 Routing Policies
- Simple Routing Policy
    - No Health Check
- Weighted Routing Policy
    - Includes Health Check
    - Used to distribute traffic across multiple EC2 instances
- Latency Routing Policy
    - Includes Health Check
    - Used to minimize latency
- Failover Routing Policy
    - Includes Health Check
    - Used to help with disaster recovery