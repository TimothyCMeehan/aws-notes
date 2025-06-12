# IAM Quick Sketch

```mermaid
flowchart TD
    A(User) --> |CLI login| B[IAM Role]
    B --> C{Policy}
    C -->|Allow| D[S3 ListBuckets]