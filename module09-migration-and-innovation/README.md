# Module-09-Migration-And-Innovation

## Learning Objectives

- Understand migration and innovation in the AWS Cloud
- Summarize the AWS Cloud Adoption Framework (AWS CAF)
- Summarize the six key factors of a cloud migration strategy
- Describe the benefits of AWS data migration solutions, such as AWS Snowcone, AWS Snowball, and AWS Snowmobile
- Summarize the broad scope of innovative solutions that AWS offers

### A. AWS Cloud Adoption Framework

Guide to companies to migrate to cloud smoothly.

[AWS Cloud Adoption Framework Link](https://d1.awsstatic.com/whitepapers/aws_cloud_adoption_framework.pdf)

Guidance was organized into 6 perspectives:

1. Business Perspectives

   - Ensure IT aligns with business needs
   - IT investment links to business results
   - Roles: Business Managers, Finance Managers, Budget Owners, Strategy Stakeholders

2. People Perspectives

   - Evaluate organizational structures and roles, new skills and prcoess requirements
   - Training & staffing
   - Roles: Human Resource, People Manager

3. Governance Perspectives

   - Business governance in the gloud
   - Roles: CIO, PM, Enterprise Architect, Business Analyst, Portfolio Managers

4. Platform Perspectives

   - Principles and patterns for implementing solutions on the cloud and migrating on-premises workload to the cloud
   - Roles: CTO, IT Managers, Solutions Architect

5. Security Perspectives

   - Ensure organization meets its security goal
   - Roles: CISO (Chief Information Security Officer), IT Security Managers, IT Security Analysts

6. Operations Perspectives

   - Define how day-to-day, month-to-month, year-to-year business is conducted
   - Roles: IT Operations Manager, IT Supports Manager

### B. Migration Strategies

6 Migration Strategies

1. Rehosting

   - lift and shift

2. Replatforming

   - lift tinker and shift

3. Retire

   - removing applications that are no longer needed

4. Retain

   - keeping some applications on the source that probably need major refactor before migrate

5. Repurchase

   - moving from traditional license to software-as-a-service license
   - i.e. CRM to salesforce

6. Refactoring / Re-Architecting

   - Redesigning an application based on cloud native features

### C. Amazon Snow Family

1 PB of data with 1 Gbps bandwith would take 100 days for migration

Amazon Snow Family is a collection of physical devices that helps data transfer physically

#### Amazon Snowcone

- 14TB, 4GB Ram, 2 CPUs

#### Amazon Snowball

Can fit into server racks

1. Snowball Edge Storage Optimized

   - 80TB HDD for block volumes and S3 compatible objects
   - 1TB SATA SSD for block volumes
   - 40 vCPU and 80GiB RAM

2. Snowball Edge Compute Optimized

   - 80TB HDD for block volumes and S3 compatible objects
   - 28TB NVMe SSD for block volumes
   - 104 vCPU, 416 GiB RAM, optional NVDIA Tesla V100 GPU

#### Amazon Snowmobile

- Up to 100PB per snowmobile
- Pulled by a container

### D. Innovation With Amazon

1. VMWara Services

   - Pre-trained AI
   - Computer Vision
   - Language recommendation
   - Forcasting

2. Amazon SageMaker

   - Quickly build, train and deploy ML models

3. Amazon Augmented AI (Amazon A2I)

4. Amazon Lex

   - Heart of Alexa
   - Build voice and chatbots

5. Amazon Textract

   - extract text and data from scanned documents

6. Amazon DeepRacer

   - reinforcement racing

7. IoT

8. Satelite - AWS Ground Station

9. Amazon Transcribe

   - text-to-speech

10. Amazon Comprehend

11. Amazon Fraud Detector
