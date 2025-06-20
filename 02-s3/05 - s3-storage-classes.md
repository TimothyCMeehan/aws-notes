# S3 Storage Classes
- Amazon S3 Standard - General Purpose
- Amazon S3 Standard - Infrequent Access (IA)
- Amazon S3 One Zone - Onfrequent Access
- Amazon S3 Glacier Instant Retrieval
- Amazon S3 Glacier Flexible Retrieval
- Amazon S3 Glacier Deep Archive
- Amazon S3 Intelligent Tiering
- Can move between classes manually or using S3 Lifecycle configurations
## S3 Durability and Availability
- Durability:
    - High durability (99.999999999%, 11 9s) of objects across multiple AZ
    - If you store 10,000,000 objects with Amazon S3, you can on average expect to incure a loss of a single object once every 10,000 years
    - Same for all storage classes
- Availability:
    - Measures how readily available a service is
    - Varies depending on storage class
    - Example: S3 standard has 99.99% availability = not available 53 minutes a year
## Amazon S3 Standard - General Purpose
- 99.99% Availability
- Used for frequently accessed data
- Low latency and high throughput
- Sustain 2 concurrent facility failures
- Use Cases: Big Data analytics, mobile & gaming applications, content distribution...
## Amazon S3 Standard - Infrequent Access (IA)
- For data that is less frequently accessed, but requires rapid access when needed
- Lower cost than S3 Standard
- 99.9% Availability
- Use Cases: Disaster Recovery, backups
## Amazon S3 One Zone - Infrequent Access
- High durability (99.999999999%) in single AZ; data lost when AZ is destroyed
- 99.5% Availability
- Use Cases: Storing secondary backup copies of on-premise data, or data you can recreate
## Amazon S3 Glacier Storage Classes
- Low-cost object storage meant for archiving / backup
- Pricing: proce for storage + object retrieval cost
- Amazon S3 Glacier Instant Retrieval
    - Millisecond retrieval, great for data accessed once a quarter
    - Minimum storage duration of 90 days
- Amazon S3 Glacier Flexible Retrieval
    - Expidited (1 to 5 minutes), Standard (3 to 5 hours), Bulk (5 to 12 hours) - free
- Amazon S3 Glacier Deep Archive - for long term storage:
    - Standard (12 hours), bulk (48 hours)
    - minimum storage duration of 180 days
## Amazon S3 Intelligent Tiering
- Small monthly monitoring and auto-tiering fee
- Moves objects automatically between Access Tiers based on usage
- There are no retrieval charges in S3 Intelligent-Tiering
- Frequent Access tier (automatic): default tier
- Infrequent Access tier (automatic): objects not accessed for 30 days
- Archive Instant Access tier (automatic): objects not accessed for 90 days
- Archive Access tier (optional): configurable from 90 days to 700+ days
- Deep Archive Access tier (optional): config. from 180 days to 700+ days

