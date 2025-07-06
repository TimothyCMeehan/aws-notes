# Well Architected Framework General Guiding Principles
- Stop guessing your capacity needs
- Test systems at production scale
- Automate to make architectural experimentation easier
- Allow for evolutionary architectures
    - Design based on changing requirements
- Drive architectures using data
- Improve through game days
    - Simulate applications for flash sale days
## AWS CLoud Best Practices - Design Principles
- Scalability: vertical & horizontal
- Disposable Resources: servers should be disposable & easily configured
- Automation: Serverless, Infrastructure as a Service, Auto Scaling...
- Loose Coupling:
    - Monolith are applications that do more and more over time, becoming bigger
    - Break it down into smaller, loosely coupled components
    - A change or failure in one component should not cascade to other components
- Services, not Servers:
    - Don't use just EC2
    - Use managed services, databases, serverless, etc.
## Well Architected Framework 6 Pillars
1. Operational Excellence
2. Security
3. Reliability
4. Performance Efficiency
5. Cost Optimization
6. Sustainability
- THey are not something to balance, or trade-offs, they're a synergy