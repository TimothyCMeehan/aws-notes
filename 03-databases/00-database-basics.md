# Database Intro
- Storing data on disk (EFS, EBS, EC2 Instance Store, S3) can have limits
- Databases let you structure your data
- You build indexes to efficiently query / search through the data
- You define relationships between datasets
- Databases are optimized for a purpose and come with different features, shapes and constraints
## Relational Databases
- Looks like Excel spreadsheets, with links between them
- Can use the SQL language to perform queries / lookups
## NoSQL Databases
- NoSQL = non-SQL = non relational databases
- NoSQL databases are purpose built for specific data models and have flexible schemas for building modern appliications
- Benefits:
    - Flexibility: easy to evolve data model
    - Scalability: designed to scale-out by using distributed clusters
    - High-performance optimized for a specific data model
    - Highly functional: types optimized for the data model
- Examples: Key-value, document, graph, in-memory, search databases
## NoSQL data example: JSON
- JSON = JavaScript Object Notation
- JSON is a common form of data that fits into a NoSQL model
- Data can be nested
- Fields can change over time
- Support for new types: arrays, etc...