# AWS Systems Manager (SSM)
- Helps you manage your EC2 and On-Premise systems at scale
- Another Hybrid AWS service
- Get operational insights about state of your infrastructure
- Suite of 10+ products
- Most important features are:
    - Patching automation for enhanced compliance
    - Run commands across an entire fleet of services
    - Store parameter configurations with the SSM Parameter Store
- Works for Linux, Windows, MacOS, Paspberry Pi OS (Raspbian)
## How Systems Manager Works
- We need to install the SSM agent onto the systems we control
- Installed by default on Amazon Linux AMI & some Ubuntu AMI
- If an instance can't be controlled by SSM, it's probably an issue with the SSM agent
- Thanks to the SSM agent, we can run commands, patch & configure our servers
## SSM Session Manager
- Allows you to start a secure shell on your EC2 and on-premise servers
- No SSH access, bastion hosts, or SSH keys needed
- No prt 22 needed (better security)
- Supports Linux, macOS, and Windows
- Send session log data to S3 or CloudWatch Logs
## SSM Parameter Store
- Secure storage for configuration and secrets
- API Keys, passwords, configurations...
- Serverless, scalable, durable, easy SDK
- Control access permissions using IAM
- Version tracking & encryption (optional)