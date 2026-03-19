# Day 5 – Creating Virtual Machines and Infrastructure Automation

## 1. Recap of Previous Session (Day 4)

In the previous session we discussed:

- What is a Server
- What is a Physical Server
- What is a Virtual Machine
- How Virtual Machines evolved
- Difference between Physical Servers and Virtual Machines
- The concept that allows creation of virtual machines (Virtualization)

We also discussed how organizations used to maintain their own **data centers**.

Modern organizations are shifting towards **cloud platforms** such as:

- AWS
- Microsoft Azure
- OpenStack

Previously even startups maintained their own data centers, but today many companies rely on cloud platforms.

---

# 2. What Will Be Covered in This Session

In this session we will learn:

- Virtual machines in a deeper way
- How to create virtual machines
- Different cloud platforms

Main platforms discussed:

- AWS
- Microsoft Azure
- On-premise environments

This helps engineers working in different organizations understand how infrastructure works.

---

# 3. Creating a Virtual Machine Using Cloud Providers

To create a virtual machine, a user sends a request to a cloud provider.

Examples of cloud providers:

- AWS
- Microsoft Azure

### Example Scenario

A person sitting in front of a laptop wants a virtual machine.

Steps:

1. Open a browser
2. Go to AWS Console
3. Request a virtual machine

In AWS terminology:

**Virtual Machine = EC2 Instance**

### Result

Once the request is processed, AWS returns:

- IP Address
- Configuration details
- Login credentials

Using these details, the user can access the virtual machine.

---

# 4. Creating a Virtual Machine in Microsoft Azure

The process is similar in Azure.

Steps:

1. Open Azure Portal
2. Request a Virtual Machine
3. Azure processes the request
4. Azure provides:

- IP Address
- VM configuration details

Both AWS and Azure follow the same basic concept.

---

# 5. Problem with Manual Creation

Creating one virtual machine manually is simple.

But imagine:

100 developers request virtual machines.

Manual process would require:

- Logging into console 100 times
- Creating VMs one by one

This becomes inefficient and time consuming.

---

# 6. DevOps Solution: Automation

DevOps focuses on **automation and efficiency**.

Instead of manual work:

Engineers write scripts to automatically create virtual machines.

---

# 7. AWS APIs

AWS provides **APIs (Application Programming Interfaces)**.

Example:

- AWS EC2 API

These APIs allow developers to interact with AWS services programmatically.

Other AWS service APIs include:

- S3 API (for storage)
- EBS API (for volumes)

---

# 8. How Automation Works

A DevOps engineer writes a script.

The script:

1. Calls the AWS EC2 API
2. Sends a request
3. AWS creates the instance
4. Script receives instance details

Example:

A script can automatically create **10 EC2 instances** at once.

Benefits:

- Saves time
- Reduces manual errors

---

# 9. API Request Requirements

To successfully create resources using APIs, three conditions must be satisfied.

### 1. Valid Request

The request must follow the correct API format.

### 2. Authentication

The user must be authenticated with AWS.

### 3. Authorization

The user must have permission to create EC2 instances.

If all three conditions are satisfied, the instance will be created.

---

# 10. Methods to Automate AWS Infrastructure

DevOps engineers automate infrastructure using several tools.

## 1. AWS CLI

AWS CLI (Command Line Interface) allows engineers to manage AWS resources using terminal commands.

Example:

Commands from the terminal can create EC2 instances.

---

## 2. Direct API Usage

Developers can interact directly with AWS APIs using programming languages.

Example:

REST APIs.

---

## 3. Python with Boto3

Python provides a library called **Boto3**.

Using Boto3, developers can:

- Make API requests
- Create EC2 instances
- Manage AWS resources

---

## 4. AWS CloudFormation (CFT)

CloudFormation allows engineers to define infrastructure using templates.

Templates describe:

- Servers
- Storage
- Networks

AWS reads the template and automatically creates the infrastructure.

---

# 11. Terraform

Terraform is another popular tool used for infrastructure automation.

### Important Difference

| Tool           | Scope       |
| -------------- | ----------- |
| AWS CLI        | AWS only    |
| AWS API        | AWS only    |
| CloudFormation | AWS only    |
| Terraform      | Multi-cloud |

Terraform supports:

- AWS
- Azure
- Google Cloud

---

# 12. AWS Cloud Development Kit (CDK)

AWS also provides **Cloud Development Kit (CDK)**.

CDK allows infrastructure to be defined using programming languages.

Benefits:

- Advanced features
- Better integration with AWS services
- Faster support for new AWS services

---

# 13. Choosing the Right Tool

The tool depends on the organization's infrastructure.

### If organization uses only AWS

Tools used:

- AWS CLI
- AWS API
- CloudFormation
- AWS CDK

### If organization uses multiple clouds

Use:

- Terraform

---

# 14. Hybrid Cloud Model

Many organizations use **Hybrid Cloud**.

This means resources are distributed across multiple cloud platforms.

Example:

- AI workloads → Google Cloud
- Databases → AWS
- Applications → Azure

Terraform works well in these scenarios.

---

# 15. Creating a Virtual Machine on AWS (UI Method)

Steps:

1. Open browser
2. Go to:
