# Cloud Computing Concepts and AWS Services Report

## 1. What is Cloud Computing?

Cloud computing means using computing resources like servers, storage, databases, and networking through the internet.

### Advantages

* Low cost
* Easy scalability
* Fast deployment
* High availability

---

## 2. Cloud Deployment Models

### Public Cloud

Cloud resources are provided by a third-party provider and shared by many customers.

**Examples:** AWS, Azure, Google Cloud

### Private Cloud

Cloud infrastructure is used by only one organization.

**Example:** Company private data center

### Hybrid Cloud

Combination of public and private cloud.

**Example:** Sensitive data in private cloud and website on AWS.

---

## 3. Cloud Service Models

### IaaS – Infrastructure as a Service

Provides virtual servers, storage, and networking.

**Example:** Amazon EC2

### PaaS – Platform as a Service

Provides a platform to develop and deploy applications without managing servers.

**Example:** AWS Elastic Beanstalk, Google App Engine

### SaaS – Software as a Service

Provides ready-to-use software through the internet.

**Examples:** Gmail, Microsoft 365

---

## 4. Core AWS Services

### Amazon EC2

Provides virtual servers to run applications.

**Uses:** Website hosting, application deployment

### Amazon S3

Provides object storage for storing files and data.

**Uses:** Backup, file storage, static websites

### Amazon VPC

Provides a private and isolated network in AWS.

**Uses:** Network security and application hosting

### Amazon RDS

Provides managed relational databases.

**Examples:** MySQL, PostgreSQL, Oracle

---

## 5. AWS Security Configuration

### MFA

MFA provides an additional security layer. MFA was enabled for the AWS Root user using an authenticator app.

### IAM

IAM manages AWS users and permissions.

An IAM admin user named `shraddha-admin` was created for regular AWS activities.

### Billing Budget

A budget named `My Zero-Spend Budget` was created with a limit of **$1.00** to monitor AWS costs.

---

## 6. AWS CLI Verification

AWS CLI was configured using the IAM admin user.

Command used:

```bash
aws sts get-caller-identity
```

The command successfully verified access using the `shraddha-admin` IAM user.

The output is saved in:

`docs/aws_cli_verification.txt`

---

## 7. Conclusion

In this task, I learned the basics of cloud computing, deployment models, service models, and important AWS services.

I also configured **MFA, IAM, AWS Budget, and AWS CLI** to create a more secure AWS environment.
