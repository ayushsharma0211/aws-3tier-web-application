## Architecture Diagram

![AWS 3-Tier Architecture](architecture-diagram.png)


# AWS 3-Tier Highly Available Web Application

## Project Overview

This project demonstrates a production-style AWS 3-Tier Web Application Architecture built using core AWS services. The infrastructure is designed with high availability, scalability, security, and monitoring best practices.

The application is deployed across multiple Availability Zones in AWS Mumbai Region and is accessible through a custom domain using Route 53.

## Live Demo

**Domain:** https://ayushproject.online

## Architecture Components

### Networking

* Custom VPC
* Public Subnets (2)
* Private Subnets (2)
* Internet Gateway
* Route Tables

### Compute

* Bastion Host
* Amazon EC2 Web Servers
* Launch Template

### Load Balancing

* Application Load Balancer (ALB)
* Target Group
* Health Checks

### Scaling

* Auto Scaling Group
* Multi-AZ Deployment

### Database

* Amazon RDS

### DNS

* Amazon Route 53
* Custom Domain Configuration

### Monitoring

* Amazon CloudWatch Dashboard
* CloudWatch Alarms

## AWS Services Used

* Amazon VPC
* Amazon EC2
* Application Load Balancer
* Auto Scaling Group
* Amazon RDS
* Amazon Route 53
* Amazon CloudWatch
* Security Groups
* Internet Gateway

## Project Screenshots

All implementation screenshots are available inside the screenshots folder.

## Skills Demonstrated

* AWS Architecture Design
* VPC Networking
* EC2 Administration
* Load Balancing
* Auto Scaling
* Route 53 DNS Management
* CloudWatch Monitoring
* Linux Administration
* Bastion Host Connectivity
* High Availability Architecture

## Author

Ayush Sharma

Cloud Engineer


----------------------------------------------------------------

## Architecture Overview

This project follows a highly available 3-tier architecture deployed across multiple Availability Zones.

User Request
|
v
Route 53
|
v
Application Load Balancer
|
v
Auto Scaling Group
|
v
EC2 Web Servers
|
v
Amazon RDS

Access Management:
Developer → Bastion Host → Private Resources

Monitoring:
CloudWatch Dashboard + CloudWatch Alarms

## Key Features

* High Availability across multiple AZs
* Load Balancing using ALB
* Auto Scaling for elasticity
* Secure Bastion Host access
* Centralized monitoring with CloudWatch
* Custom Domain using Route 53
* Production-style AWS deployment

## Project Workflow

1. User accesses the application using a custom domain.
2. Route 53 resolves the domain to the Application Load Balancer.
3. ALB distributes traffic across healthy EC2 instances.
4. Auto Scaling Group maintains desired capacity.
5. EC2 instances serve application content.
6. CloudWatch monitors infrastructure metrics.
7. Bastion Host provides secure administrative access.

## Repository Structure

aws-3tier-web-application/
│
├── index.html
├── README.md
├── screenshots/
│ ├── 01-vpc-overview.png
│ ├── 02-public-subnet-az1.png
│ ├── ...
│ └── 31-deployment-and-verification.png

## Project Outcome

Successfully designed and deployed a highly available AWS 3-Tier Architecture using industry-standard cloud services and best practices.

This project demonstrates practical experience with networking, compute, load balancing, auto scaling, monitoring, security, and DNS management within AWS.


