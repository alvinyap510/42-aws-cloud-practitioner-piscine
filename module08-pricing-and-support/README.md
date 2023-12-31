# Module-08-Pricing-And-Support

## Learning Objectives

- Describe AWS pricing and support models
- Describe the AWS Free Tier
- Describe key benefits of AWS Organizations and consolidated bills
- Explain the benefits of AWS Budget
- Explain he nebefits of AWS Cost Explorer
- Explain the primary benefits of the AE Pricing Calculator
- Distinguish various AWS Support Plans
- Describe the benefits of AWS Marketplace

### A. AWS Free Tier

#### 3 Types of free tier

- Always Free
- 12 months free
- Trials

Lambda

- Free 1 million invocations => Always free

S3

- Free 12 months for up to 5GB of storage

Lightsail

- 1 month trial of up to 750 hours of usage

Others

- SageMaker
- ComprehendMedical
- DynamoDB
- SNS
- Cognito

### B. AWS Pricing Concepts

#### How AWS pricing works

1. Pay for what you use

   - No long term contract
   - No complex license

2. Pay less when you reserve

   - Significant discount up to 72%
   - Commit a certaina usage

3. Pay less with volume-based discounts when you use more

   - Per unit cost decreases when you use more
   - ie: the more S3 storage you use, the less per GB you pay for

#### AWS Pricing Calculator

- [AWS Calculator Link](https://calculator.aws/#/)
- Create estimation for the cost of usage
- Save and send it as a link
- Compare which region / which instance type save the most cost

#### AWS Pricing Examples

1. AWS Lambda (Pay Less When Reserve)
   - Charged based on number of requests
   - 1 million free requests and up to 3.2 million seconds of compute time
   - Compute Savings Plan: Lower compute costs in exchange for a commitment of consistent usage (1 year / 3 years)
2. Amazon EC2
   - Pay only the compute time while instance running
   - Use spot instances to save up to 90%
   - Savings Plan and Reserved Instance option available
3. Amazon S3
   - Pay storage used
   - Charge rate based on objects stored size, class, and how long it was stored
   - Pay for requests for the information (say website hosting, will pay based on visitor's request)
   - No cost transfer between different Amazon S3 buckets
   - No cost transfer between Amazon S3 and other services within the same region
   - Pay for data transfer into and out of Amazon S3
   - No Cost for daya transferred into Amazon S3 and out to CloudFront
   - Management and replication: Pay for the storage management features that you have enabled on account's Amazon S3 buckets (inventory, analytics, object tagging)

### C. AWS Billing Dashoard

- Search billing to go to Dashboard
  - compare month-to-date with previous month
  - forcast of next month
  - split by services
  - view free-tier
  - cost explorer
  - create budgets
  - purchase and manage savings plan
  - publis AWS Cost and Usage Reports

### D. Consolidated Bill

- Default number of allowed AWS ccounts in an organization is 4
- Consolidate bill to the organization owner
- Bulk discount
- Share reserved instances and bulk discount pricing

### E. AWS Budgets

- Navigate to billing => click budget => set budget
- Update 3 times a day
- Set custom budgets for cost and usage
- Get notified when exceed or forecasted to exceed

### F. AWS Cost Explorer

- Search cost explorer
- Console based service
- 12 months of historical data
- create tags to organize certain projects together
- tag is key-value pair
- filter by tag
- generate custom reports and save it

### G. AWS Support Plans

1. Basic Support

   - no cost
   - 24/7 customer service
   - documentation
   - whitepapers
   - support forums
   - AWS Trusted Advisor
   - AWS Personal Health Dashboard

2. AWS Developer Support

   - Email access to customer service
   - Best Practice Guidance
   - Client-side diagnostic tools
   - Building-block architecture support

3. AWS Business Support

   - Advance Trusted Advisor => Full set best practice checks
   - Direct phone access to cloud support engineer
   - Infrastructure event management => launching etc.
   - Limited support for third-party software, such as common operating systems and application stack components

4. Enterprise On-Ramp

   - 30 minute response time for business critical workload
   - access to Technical Account Managers (TAMs)
   - Cost optimization workshop (once per year)
   - concierge support for billing and account assistance
   - consultative review and architecture guidance (once per year)
   - infrastructure event management (once per year)
   - support automation workflows

5. AWS Enterprise

   - 15 minute response time for business critical workload
   - Designated Technical Account Manager (TAMs)
   - Operation Review / Well-Architected Review

- Six Pillars of Well-Architected Framework

  - Operational Excellence
  - Security
  - Reliability
  - Performance Efficiency
  - Cost Optimization
  - Sustainability

### H. AWS Marketplace

- Digital Catalog
- Third-party software
- Listed by independent software vendors
- Flexible pricing plans
- exp: one-click deployment
- categories:
  - Infrastructure Softwares
  - DevOps
  - Data Products
  - Professional Services
  - Business Applications
  - Machine Learning
  - Industries
  - IoT
