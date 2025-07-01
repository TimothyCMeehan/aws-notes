# Amazon CloudWatch Logs
- CloudWatch Logs collect logs from:
    - Elastic Beanstalk collection of logs from application
    - ECS: collection from containers
    - AWS Lambda: collection from function logs
    - CloudTrail based filter
    - CloudWatch log agents: EC2 machines or on-prem servers
    - Route53: Log DNS queries
- Enable real-time monitoring of logs
- Adjustable CloudWatch Logs retention
## CloudWatch Logs for EC2
- By default, no logs from EC2 instance will go to CloudWatch
- You need to run a CloudWatch agent on EC2 to push the log files you want
- Make sure IAM permissions are correct
- The CloudWatch log agent can be setup on-prem too