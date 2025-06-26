# Amazon SQS - Simple Queue Service
## What's a queue?
- Allows Application layers to scale independently based on demand
## Standard Queue
- Oldest AWS offering (over 10 years old)
- Fully managed service (serverless), used to decouple applications
- Scales from 1 message per second to 10,000s per second
- Default retention of messages: 4 days, maximum of 14 days
- No limit to how many messages can be in the queue
- Messages are deleted after they're read by consumers
- Low latency (<10ms on publish and receive)
- Consumers share the work to read messages & scale horizontally
## FIFO Queue
- FIFO = First In First Out (ordering messages in the queue)
- Messages are processed in order by the consumer
