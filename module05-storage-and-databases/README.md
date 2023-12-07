# Module-05-Storage-And-Databases

## Learning Objectives

- Summarise the basic concepts of storage and databases
- Describe the benefits of Amazon Elastic Block Store (Amazon EBS)
- Describe the benefits of Simple Storage Service (Amazon S3)
- Describe the benefits of Amazon Elastic File System (Amazon EFS)
- Summarise various storage solutions
- Describe the benefits of Amazon Relational Database Service (Amazon RDS)
- Describe the benefits of Amazon DynamoDB
- Summarize various database services

### A. Instance Stores and Amazon Elastic Block Store (Amazon EBS)

#### Block Level Storage

- Can used as databases, enterprise softwares and file systems
- Labtop and computer uses block levek storage: hard drive
- Depends on instance type, it might have Instance Store Volumes (Local Storage), write to it as normal hard drive
- Since it is attached to the instance, once instance stopped, all info will be deleted
- To store: temporary files, scratch datas

#### Amazon Elastic Block Store

- Virtual Hard Drives
- Attach to EC2 instances
- Functions similar to an external hard disk
- Snapshots: Incremental backups of the data

### B. Amazon Simple Storage Service (Amazon S3)

- Data stored as objects
  - file == object
  - file directory == bucket
- Can version objects
- Multiple buckers = tiers / class

1. Amazon S3 Standard

- Frequent accessed data
- Stored in at least 3 facilities
- 99.999999999 % Durability
- Amazon Static Website Hosting
- upload inside a bucket
- check => host as static website

2. Amazon S3 Standard-Infrequent Access (S3 Standard -IA)

- Infrequently accessed data
- Lower storage price but higher retrieval price
- used for data that is accessed less frequently but when needed need to be accessed rapidly

3. Amazon S3 One Zone-Infrequent Access

- Only stores data in a single availability zone (compliance issue?)
- Lower storage price than Standard-IA

4. Amazon S3 Life Cycle Policies

- Auto matic move data between different S3 services

Object Storage:

- Contains key, metadata and data

5. Amazon S3 Intelligent Tiering

- Unknown or changing access patterns
- Requires a small montuly monitoring and automation fee per object

6. Amazon S3 Glacer Instant Retrieval

- Archieved data that need immediate access
- Within few milliseconds

7. Amazon S3 Glacier Flexible Retrieval

- example: audit data
- Low data archieving cost
- retrieve objects within a few minutes to hours
- 1 munutes - 12 hours

8. Amazon S3 Glacier Deep Archive

- Lowest costs
- Retrieve within 12 hours - 48 hours
- accessed once or twice in a year
- replicated and stored at least three geographically dispersed availability zone

9. Amazon S3 Outposts

- On premises AWS Outposts
- Create S3 Bucket on AWS Outposts

Elastic Block Storage vs S3

| EBS                              | S3                     |
| -------------------------------- | ---------------------- |
| Up to 16TiB                      | Unlimited Storage      |
| Survive Termination of Instances | Objects Upto 5 TB      |
| Solid State by Default           | 99.999999999 % Durable |
| HDD by Option                    | Worm                   |

Example: Photo Analysis

- Amazon S3
- Web enabled
- Regionally distributed
- Cost savings

Object Storage vs Block Storage

- Block storage allow files to be updated only the parts that has changes

If constant read, write, update => choose EBS

### C. Amazon Elastic File System (Amazon EFS)

- Shared file systems accross different applications
- Allow multiple instances to access data in the EFS at the same time
- Linux File Systems
- Regional resource
- On-premise servers => access EFS via AWS Direct Connect
- Compare EBS:
  - EBS Volumes attached to EC2 instances, need to be at the same AZ
  - EBS does not automatically scaled

### D. Amazon Relational Dataservice Service (Amazon RDS)

Suports:

- Amazon Aurora
- MySQL
- PostgreSQL
- Oracle Database
- MariaDB
- Microsoft SQL Server

Migrate to Clould

- Lift and shift

Amazon RDS

- Run relational database on the cloud
- Can intergrate with Lambda
- Automated Patching
- Backups
- Redundancy
- Failover
- Disaster recovery

Amazon Aurora

- Amazon's own relational database
- Compatible with MySQL and PostgreSQL
- 5x faster than MySQL and 3x faster than PostgreSQL
- 1 / 10th of commercial databases
- 6 copies replicated at any given time
- continuous backup to S3
