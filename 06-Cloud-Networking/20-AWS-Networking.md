# AWS Networking

## VPC

VPC stands for Virtual Private Cloud.

A logically isolated network inside AWS.

---

## Components of VPC

- Subnets
- Route Tables
- Security Groups
- NACLs
- Internet Gateway
- NAT Gateway

---

## Public Subnet

Resources can access the Internet.

Examples:
- Web Servers
- Load Balancers

---

## Private Subnet

Resources are not directly accessible from the Internet.

Examples:
- Databases
- Internal Applications

---

## Internet Gateway

Provides Internet access to public resources.

---

## NAT Gateway

Allows private resources to access the Internet without exposing them publicly.

---

## Security Groups

Acts as a virtual firewall for EC2 instances.

Characteristics:
- Stateful

---

## Network ACL (NACL)

Acts as a firewall at subnet level.

Characteristics:
- Stateless

---

## Security Group vs NACL

| Feature | Security Group | NACL |
|----------|---------------|-------|
| Level | Instance | Subnet |
| Stateful | Yes | No |
| Allow Rules | Yes | Yes |
| Deny Rules | No | Yes |

---

## VPC Flow

Internet

↓

Internet Gateway

↓

Public Subnet

↓

Application Server

↓

Private Subnet

↓

Database Server
