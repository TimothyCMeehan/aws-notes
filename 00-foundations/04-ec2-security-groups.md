# EC2 Security Groups
- Security Groups are the fundamental of network security in AWS
- control how traffic is allowed into or out of EC2 Instances
- contain only allow rules
- can reference by IP or by security group
- act as a 'firewall' on EC2 instances
- They regulate:
    - Access to Ports
    - Authorize IP ranges - IPv4 and IPv6
    - Control of inbound network (from other to the instance)
    - Control of outbound network (from the instance to other)
## Important Considerations
- Can be attached to multiple instances
- Locked down to a region / VPC combination
- Does live 'outside' the EC2 instance - if traffic is blocked, the EC2 instance won't see it
- It's good to maintain one seperate security group for SSH access
- If your application is not accessible (time out), then it's a security group issue
- If your application geives a 'connection refused' error, then it's an application error or it's not launched
- All inbound traffic is blocked by default
- All outbound traffic is authorized by default
## Classic Ports
- 22 = SSH (Secure Shell) - log inot a Linux instance
- 21 = FTP (File Transfer Protocol) - upload files using SSH
- 22 = SFTP (Secure File Transfer Protocol) - upload files using SSH
- 80 = HTTP - access unsecured websites
- 443 = HTTPS - access secured websites
- 3389 = RDP (Remote Desktop Protocol) - log into a Windows instance