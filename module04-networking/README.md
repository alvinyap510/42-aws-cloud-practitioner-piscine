# Module-04-Global-Networking

## Learning Objectives

- Describe the basic concepts of Networking
- Difference between public and private networking
- Explain Virtual Private Gateway
- Explain Virtual Private Network

### A. Amazon Virtual Private Cloud (VPC)

- A logically isolated section where user define
- Can be public facing (with internet access) and private facing (without internet acccess)
- Private facing example: databases / application servers
- Together pulic + private - known as subnets - determined by IPs within the VPC
- Everything is EC2 Instances or ELP are inside the VPC
- Public Facing VPC
  ![Public Facing VPC](public-facing-vpc.png)

  - Install internet gateway

- Private Facing VPC
  ![Private Facing VPC](private-facing-vpc.png)

  - Install virtual private gateway
  - Allows private network to connect to virtual private gateway via VPN

- AWS Direct Connect
  ![AWS Direct Connect](aws-direct-connect.png)
  - Private direct fibre connect from from data center to AWS
