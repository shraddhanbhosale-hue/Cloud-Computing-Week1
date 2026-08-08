# Cloud Computing Concepts and AWS Services Report

## 1. Introduction to Cloud Computing

Cloud computing is the delivery of computing resources such as servers, storage, databases, networking, and software over the internet. It allows users and organizations to access IT resources without owning and maintaining physical hardware.

Cloud providers generally offer resources using flexible and pay-as-you-go pricing models, which can help organizations reduce infrastructure costs and scale resources according to demand.

Major cloud providers include:

* Amazon Web Services (AWS)
* Microsoft Azure
* Google Cloud Platform (GCP)

### Advantages of Cloud Computing

* Cost optimization
* Scalability
* High availability
* Flexibility
* Faster deployment
* Reduced hardware maintenance

---

# 2. Cloud Deployment Models

## Public Cloud

Public cloud is a cloud deployment model in which computing resources are owned and managed by a third-party cloud provider and are made available to multiple customers over the internet.

Examples:

* Amazon Web Services (AWS)
* Microsoft Azure
* Google Cloud Platform (GCP)

### Advantages

* Low initial infrastructure cost
* Easy scalability
* No need to maintain physical hardware
* Quick resource provisioning

### Disadvantages

* Less direct control over the underlying infrastructure
* Requires proper security and access management

## Private Cloud

Private cloud is a cloud environment dedicated to a single organization. The organization has greater control over its infrastructure, security, and resources.

Examples:

* Organization-owned private data centers
* VMware-based private cloud environments

### Advantages

* Greater control
* Customizable infrastructure
* Suitable for organizations with specific security requirements

### Disadvantages

* Higher setup and maintenance costs
* Requires skilled IT staff
* Infrastructure management can be complex

## Hybrid Cloud

Hybrid cloud combines public and private cloud environments. It allows organizations to use both environments according to their requirements.

For example, an organization can keep sensitive data in a private environment while hosting a public-facing application using AWS.

### Advantages

* Flexible infrastructure
* Better control over sensitive workloads
* Cost optimization
* Easy workload distribution

---

# 3. Cloud Service Models

## Infrastructure as a Service (IaaS)

IaaS provides virtualized computing resources such as servers, storage, and networking over the internet.

### Provider manages:

* Physical hardware
* Data centers
* Networking infrastructure
* Virtualization

### User manages:

* Operating system
* Applications
* Data
* Configuration

### Examples

* Amazon EC2
* Microsoft Azure Virtual Machines
* Google Compute Engine

## Platform as a Service (PaaS)

PaaS provides a managed platform for developing, testing, and deploying applications without requiring developers to manage the underlying infrastructure.

### Provider manages:

* Servers
* Operating system
* Runtime environment
* Infrastructure

### User manages:

* Application code
* Application data

### Examples

* AWS Elastic Beanstalk
* Google App Engine
* Heroku

## Software as a Service (SaaS)

SaaS provides ready-to-use software applications over the internet. Users generally do not need to manage the underlying infrastructure.

### Examples

* Gmail
* Microsoft 365
* Salesforce

---

# 4. Core AWS Services

## Amazon EC2 (Elastic Compute Cloud)

Amazon EC2 provides resizable virtual computing capacity in the AWS cloud. Users can launch virtual servers called instances and configure them according to their application requirements.

### Features

* Resizable computing capacity
* Multiple operating system choices
* Scalable resources
* Flexible pricing options

### Uses

* Website hosting
* Application deployment
* Development and testing
* Running backend applications

## Amazon S3 (Simple Storage Service)

Amazon S3 is an object storage service used to store and retrieve data from anywhere through the internet.

### Features

* Highly durable storage
* Scalable storage capacity
* Access control and security features
* Support for different storage classes

### Uses

* Backup and recovery
* File storage
* Data storage
* Static website hosting

## Amazon VPC (Virtual Private Cloud)

Amazon VPC allows users to create a logically isolated virtual network within AWS. Users can control networking components such as IP addresses, subnets, routing, and network access.

### Features

* Subnets
* IP address ranges
* Route tables
* Security groups
* Network access control

### Uses

* Secure application hosting
* Network segmentation
* Controlling access to AWS resources

## Amazon RDS (Relational Database Service)

Amazon RDS is a managed relational database service that simplifies the setup, operation, and scaling of relational databases.

### Supported database engines include:

* MySQL
* PostgreSQL
* Oracle
* Microsoft SQL Server

### Features

* Automated backups
* Database monitoring
* High availability options
* Easier database administration

---

# 5. AWS Security Configuration

## Multi-Factor Authentication (MFA)

Multi-Factor Authentication adds an additional layer of security to an AWS account. In this setup, MFA was enabled for the AWS root user using an authenticator application.

MFA helps protect the account even if the account password is compromised.

## IAM (Identity and Access Management)

AWS IAM is used to manage identities and permissions for accessing AWS resources.

For this task, an IAM administrative user named `shraddha-admin` was created for regular AWS activities instead of using the root account.

### Security Best Practices

* Avoid using the root account for daily activities.
* Use IAM identities for regular AWS operations.
* Enable MFA.
* Grant only the permissions required for a specific task whenever possible.
* Protect AWS access keys and never publish them in a public repository.

## Billing Budget and Cost Monitoring

An AWS budget named `My Zero-Spend Budget` was configured to monitor AWS spending.

The configured budget amount is **$1.00**, and the current amount used is **$0.00**.

This helps monitor AWS costs and provides an early warning if spending approaches or exceeds the configured threshold.

---

# 6. AWS CLI Verification

The AWS CLI was installed and configured using the IAM administrative user's credentials.

The following command was used to verify the AWS CLI configuration:

```bash
aws sts get-caller-identity
```

The command successfully returned the identity associated with the `shraddha-admin` IAM user.

The verification output is documented separately in:

`docs/aws_cli_verification.txt`

Sensitive account information and credentials should not be publicly exposed in the repository.

---

# 7. Conclusion

This task provided a practical introduction to cloud computing and Amazon Web Services. I learned about public, private, and hybrid cloud deployment models and the IaaS, PaaS, and SaaS service models.

I also explored important AWS services including Amazon EC2, Amazon S3, Amazon VPC, and Amazon RDS.

As part of the hands-on security setup, I enabled MFA for the root account, created an IAM administrative user, configured AWS CLI access, and created a billing budget for cost monitoring.

These activities provided a foundation for securely using AWS for future cloud computing and DevOps projects.
