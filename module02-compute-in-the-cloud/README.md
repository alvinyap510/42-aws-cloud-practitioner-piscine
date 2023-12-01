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

A. Amazon Elasctic Compute Cloud

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
