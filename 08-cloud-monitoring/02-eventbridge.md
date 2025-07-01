# Amazon EventBridge (formerly CloudWatch Events)
- Schedule: Cron Jobs (scheduled scripts)
- Event Pattern: Event rules to react to a service doing something
- Trigger Lambda functions, send SQS/SNS messages...
## Event Bus
- Default Event Bus: from AWS services
- Partner Event Bus: from AWS SaaS partners
- CUstom Event Bus: from custom apps
## Other Features
- Schema REgistry: mdel event schema
- You can archive events (all/filter) sent to an event bus (indefinitely or set period)
- Ability to replay archived events