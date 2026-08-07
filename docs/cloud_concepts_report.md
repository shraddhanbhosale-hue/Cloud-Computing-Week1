# Cloud Computing Concepts and AWS Services Report

## 1. Introduction to Cloud Computing

Cloud computing is the delivery of computing resources such as servers, storage, databases, networking, and software through the internet. It allows users to access IT resources without owning physical hardware.

Cloud providers offer resources on a pay-as-you-go basis, which helps organizations reduce cost and improve scalability.

Major cloud providers:
- Amazon Web Services (AWS)
- Microsoft Azure
- Google Cloud Platform (GCP)

### Advantages of Cloud Computing
- Cost reduction
- Scalability
- High availability
- Flexibility
- Faster deployment


# 2. Cloud Deployment Models

## Public Cloud

Public cloud is a cloud model where resources are owned and managed by third-party cloud providers and are available to multiple customers over the internet.

Examples:
- AWS
- Microsoft Azure
- Google Cloud

Advantages:
- Low initial cost
- Easy scalability
- No hardware maintenance

Disadvantages:
- Less control over infrastructure
- Security concerns for sensitive data


## Private Cloud

Private cloud is a cloud environment dedicated to only one organization. The organization has complete control over its infrastructure and resources.

Examples:
- Company private data centers
- VMware private cloud

Advantages:
- Better security
- More control
- Customization

Disadvantages:
- Expensive setup
- Requires maintenance


## Hybrid Cloud

Hybrid cloud combines both public and private cloud environments. It allows organizations to keep sensitive data in a private cloud while using public cloud resources for other applications.

Advantages:
- Flexible infrastructure
- Better security
- Cost optimization

Example:
A company can store confidential customer information in a private cloud and host its website on AWS public cloud.


# 3. Cloud Service Models

## Infrastructure as a Service (IaaS)

IaaS provides virtualized computing resources such as servers, storage, and networking over the internet.

The cloud provider manages:
- Physical hardware
- Networking
- Data centers

The user manages:
- Operating system
- Applications
- Data

Examples:
- Amazon EC2
- Microsoft Azure Virtual Machines
- Google Compute Engine


## Platform as a Service (PaaS)

PaaS provides a platform that allows developers to build, test, and deploy applications without managing the underlying infrastructure.

The provider manages:
- Servers
- Operating system
- Runtime environment

The user manages:
- Application code
- Data

Examples:
- AWS Elastic Beanstalk
- Google App Engine
- Heroku


## Software as a Service (SaaS)

SaaS provides ready-to-use software applications through the internet.

Users do not manage infrastructure; they only use the application.

Examples:
- Gmail
- Microsoft 365
- Salesforce


# 4. Core AWS Services

## Amazon EC2 (Elastic Compute Cloud)

Amazon EC2 is a cloud service that provides virtual servers to run applications.

Features:
- Resizable computing capacity
- Multiple operating system choices
- Scalable resources
- Pay-as-you-go pricing

Uses:
- Website hosting
- Application deployment
- Software testing


## Amazon S3 (Simple Storage Service)

Amazon S3 is an object storage service used to store and retrieve data from anywhere.

Features:
- Highly durable storage
- Unlimited scalability
- Secure data storage

Uses:
- Backup storage
- File storage
- Static website hosting


## Amazon VPC (Virtual Private Cloud)

Amazon VPC allows users to create a private and isolated network environment inside AWS.

Features:
- Create subnets
- Configure IP addresses
- Control network access
- Use security groups

Uses:
- Secure application hosting
- Network management


## Amazon RDS (Relational Database Service)

Amazon RDS is a managed database service that makes it easy to set up and operate relational databases.

Supported databases:
- MySQL
- PostgreSQL
- Oracle
- SQL Server

Features:
- Automated backups
- High availability
- Database scaling


# 5. AWS Security Configuration

## Multi-Factor Authentication (MFA)

MFA provides an additional security layer by requiring verification through another device along with the password.

## IAM (Identity and Access Management)

IAM allows users to manage access permissions for AWS resources.

Best practice:
- Do not use the root account for daily activities.
- Use IAM users with required permissions.

## Billing Alarm

Billing alarms help monitor AWS spending and notify users when costs exceed a selected limit.


# Conclusion

This task helped me understand cloud computing fundamentals, cloud deployment models, cloud service models, AWS core services, and AWS security best practices.