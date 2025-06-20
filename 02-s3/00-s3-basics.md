# Amazon S3 Use Cases
- Backup and Storage
- Disaster Recovery
- Archive
- Hybrid Cloud storage
- Application hosting
- Media hosting
- Data lakes & big data analytics
- Software delivery
- Static website
## Buckets
- Amazon S3 allows people to store objects (files) in 'buckets' (directories)
- Buckets must have a globally unique name (across all regions and all accounts)
- Buckets are defined at the region level
- Naming convention
    - No uppercase, No underscore
    - 3-63 characters long
    - Not an IP
    - Must start with lowercase letter or number
    - Must NOT start with the prefix xn--
    - Must NOT end with the suffix -s3alias
## Objects
- Objects (files) have a key
- The key is the FULL path:
- The key is composed of prefix + object name
    - s3://my-bucket/my_folder1/another_folder/my_file.txt
- There's no concept of "directories" within buckets (although the UI will trick you to think otherwise)
- keys are just very long anmes that contain slashes
- Object values are the content of the body:
    - Max Object Size is 5TB (5000GB)
    - If uploading more that 5 GB, must use "multi-part upload"
- Metadata (list of text key / value pairs - system or user metadata)
- Tags (Unicode key / value pair - up to 10) - useful for security / lifecycle
- Version ID (if versioning is enabled)
## AWS Storage Gateway
- Brdge between on-premise data and cloud data in S3
- Hybrid storage service to allow on-premise storage solutions to seamlessly use the AWS Cloud
