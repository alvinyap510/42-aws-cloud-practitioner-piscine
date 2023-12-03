# Module-02-Compute-In-The-Cloud

## Learning Objectives

- Benefits of EC2 at a basic level
- Different EC2 instances
- Billing options of EC2
- Benefits of AWS EC2 Auto Scaling
- Benefits of AWS EC2 Elastic Load Balancing
- Demo EC2 Elastic Load Balancing
- Compare Amazon Simple Notifications System (Amazon SNS) and Amazon Simple Queue System(Amazon SQS)
- Summarize additional Amazon compute options

## Notes

### A. Amazon Elasctic Compute Cloud

- Better known as EC2
- Equivalent
  - Google Compute Engine
  - Azure Virtual Machines
- Able to configure CPU, Memory and Storage
- Pricing Model: Pay for what you use
- EC2 only pay for active instances, do not pay for stopped and terminated instances
- Hypervisor distribute resources between different virtual machines (instances)

B. Hypervisor (Coordinating Multitenancy)

- Software, Firmware or Hardware that allows multiple VMs to share resources of a physical machine's resources (CPU, RAM, Memory)
- Isolating different VMs
- An EC2 instances is not aware of another EC2 instances that shares a host machine

  1. Type 1 (Bare-Metal Hypervisors)

     - Hardware

  2. Type 2 (Hosted Hypervisors)

     - Programme

C. Amazon EC2 Configurations

- OS: Windoes, Linux
- Software
- Databases
- Third-party Softwares
- Resizable (Vertical Scaling)

D. Types of EC2 Instances

- Grouped by instances families

  - I. General Purpose

    - Balanced resources
    - Diverse workloads
    - Used as: Web Servers, Code Repositories

  - II. Compute Optimized

    - Gaming Server
    - Scientific Modelling
    - High Performance Computing
    - Parallel processing, advanced networking, large-scale data handling, financial modelling

  - III. Memory Optimized

    - Memory intensive tasks

  - IV. Accelarated Computing

    - Floating point calculations
    - Graphics processing
    - Data pattern matching
    - Utilizaes hardware accelators

  - V. Storage Optimized

    - Workloads that require high performance of locally stored data
    - Distributed File-Systems / Data-Warehousing Applications / High-Frequency online transaction processing (OLTP) systems
    - Data-Warehousing: refers to the process of aggregating large volume of data into a single / central place, for analysis or querying

<details>
<summary>E. Amazon EC2 Billing Options
</summary>
  <details>
    <summary>On-Demand Pricing</summary>
  
- Only pay for the duration the instance  runs for
- Per Hour / Per Second
- No long term commitment
- No upfront payment
  
  </details>
  
  <details>
    <summary>Savings Plan</summary>
  
- Low Price In Exchange for Consistent
- Savings up to 72%
  
  </details>
  
  <details>
    <summary>Reserved Instances</summary>
  
- Upfront payment
  - All
  - Partial
  - No Upfront
  - Savings up to 75%
  
  </details>
  
  <details>
    <summary>Spot Instances</summary>
  
  - Up to 90% savings
  - Request spare AWS computing capacity
  - Can reclaim anytime
  - 2 minute notifications to reclaim
  
  </details>
  
  <details>
    <summary>Dedicated Host</summary>
  
  - Fully dedicated physical servers
  - Most Expensive
  
  </details>

</ul>
</details>

### F. Scaling Amazon EC2

#### Amazon EC2 Auto Scaling

- Enable developer to automatically add or remove Amazon EC2 instances in response to changing application demand

  - Dynamic Scaling
  - Predictive Scaling

- Settings

  - Minimum
  - Desired
  - Maximum (Scale As Need)

### G. Directing Traffic with Elastic Load Balancing

#### Load Balancing

Computing technique to distribute workloads accross multiple computing resources.

- Contexts
  - Server load balancing
  - network load balancing
- Types
  - Hardware load balancing
  - Sofrware load balancing
- Algorithms
  - Round Robin
  - Least Connections
  - IP Hash
- Applications
  - Webservers
  - Databases
  - Clould Services
  - Virtual Networks

#### AWS Elastic Load Balancing (AWS ELB)

Functions like a host, directing customers to different cashiers who are free.

Ensure even distribution between EC2 instances.

- Regional Construct
- Decoupled Architecture
- Works together with EC2 Auto-Scaling to manage instances
- Also orchestra between frontend instances and backend intances

### H. Messaging and Queuing

Similar to an order board on a restaurant, where chasier receives orders, and the orders will be posted to the order board for kitchen to process it.

- If cachier directly talks to the barista, then it is called a tightly coupled application
- Alternatively, a loosely coupled architecture ensures that a single failure doesn't causes cascading collapse

#### Message Queue

When Application A tries to talk to Application B, a message queue acts as a buffer so that when Application B goes down, the requests are still queued with the buffer and eventually get processed when application B spin up again.

- #### Amazon Simple Queue Service (Amazon SQS)

  - Send, store and receive messages between software components at any volume
  - Data contained in SQS is called a payload
  - Messages are stored until they are processed

- #### Amazon Simple Notification Service (Amazon SNS)

  - Can also send out notifications to end user
  - Public-Subsribe Model
  - Subscribers can be: Mobile pushes, SMS, emails, endpoints, SQS queues, Lambda functions, Webhooks

#### Components of an Applications

- Databases
- Servers
- Interface
- Business Logics

Monolithic vs Microservices Architecture
