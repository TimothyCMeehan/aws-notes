# Scalability & High Availability
- Scalability means that an application / system can handle greater loads by adapting.
- There are two kinds of scalability:
    - Vertical Scalability
    - Horizontal Scalability (= elasticity)
- Scalability is linked but different to High Availability
## Vertical Scalability
- Vertical Scalability means increasing the size of the instance
- For example, your application runs on a t2.micro
- Scaling that application vertically means running it on a t2.large
- Vertical scalability is very common for non distributed systems, such as databases.
## Horizontal Scalability
- Horizontal Scalability means increasing the number of instances / systems for your application
- Horizontal scaling implies distributed systems.
- This is very common for web applications / modern applications
- It's easy to horizontally scale thanks to the cloud offerings such as EC2 with Auto Scaling Groups and Load Balancers
## High Availability
- High Availability usually goes hand and hand with horizontal scaling
- High availability means running your application / system in at least 2 Availability Zones
- The goal of High Availability is to survive a data center loss (disaster)
- achieved with Auto Scaling Group multi AZ and Load Balancer multi AZ
## Scalability vs Elasticity vs Agility
- Scalability: ability to accomodate a larger load by making the hardware stronger (scaling up), or by adding nodes (scaling out)
- Elasticity: once a system is scalable, elasticity means that there will be some 'auto-scaling' so that the system can scale based on the load. This is 'cloud friendly'; pay-per-use, match demand, optimize costs
- Agility: new IT resources are only a click away, which means that you reduce the time to make resources available (from weeks to minutes)


