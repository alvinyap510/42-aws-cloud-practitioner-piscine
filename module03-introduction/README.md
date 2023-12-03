# Module-03-Global-Infrastructure-And-Reliability

## Learning Objectives

- Summarize the benefits of AWS Global Infrastructure
- Describe the basic concept of Availability Zones
- Describe the benefits of Amazon CloudFront and edge locations
- Compare different methods for provisioning AWS Services

### A. AWS Global Infrastructure

- no information will move from 1 region to another without the prior approval of user
  - regional data sovereignty
  - example: government regulations
- choose regions
  1. compliance
  2. proximity
  3. feature availability
  4. pricing

### B. Availability Zones

- Each availability zone has one or more data centers
- Each AWS region contain multiple availabilituy zones
- Best practice: run at least 2 instances in different AZs
- AWS Elastic Load Balancing is a regional construct

### C. AWS Edge Locations

- Utilizes content delivery networks (CDNs) to cache a copy near some edge locations
- CDN: Amazon CloudFront
- DNS: Amazon Route 53
- On-Premises: AWS Outposts

### D. How to Provision AWS Resources

- In AWS, everything is an API call.
- Example:
  - Create AWS Instances
  - Deploy AWS Lambda Functions

#### Interacting with AWS Services

- AWS Management Console
  - Browser based
  - Visual
  - Include wizards and automated workflows
  - Tasks: test environment, view bills, monitoring, work with non-technical resources
- AWS CLI
  - Interacting using terminal
  - Interact programmatically
- AWS SDK
  - Interact through various programming languages
- AWS Elastic Beanstalk
  - Provide application code and desired configuration
  - Beanstalk will configure automatically
  - Focus on the business application, not the infrastructure
- AWS CloudFormation
  - Infrastucture as code tool
  - Using something like json / yaml
  - supports: storage, database, analytics, machine learnings etc.
  - manages all the APIs for user
