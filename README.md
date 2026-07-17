Top 20 AWS CLI Commands

## Table of Contents

* Introduction
* Prerequisites
* Top 20 AWS CLI Commands
* AWS CLI Cheat Sheet
* Best Practices
* Resources
* License

---

# Introduction

The **AWS Command Line Interface (AWS CLI)** is a unified tool that allows you to manage AWS services directly from the terminal. With AWS CLI, you can automate cloud operations, deploy infrastructure, manage storage, monitor resources, and interact with AWS services efficiently.

---

# Prerequisites

Before using these commands, ensure you have:

* An AWS account
* AWS CLI installed
* IAM user with programmatic access
* Configured AWS credentials

Verify installation:

```bash
aws --version
```

Configure AWS CLI:

```bash
aws configure
```

---

# Top 20 AWS CLI Commands

## 1. Check AWS CLI Version

```bash
aws --version
```

---

## 2. Configure AWS CLI

```bash
aws configure
```

---

## 3. List S3 Buckets

```bash
aws s3 ls
```

---

## 4. Create an S3 Bucket

```bash
aws s3 mb s3://my-bucket-name
```

---

## 5. Upload a File to S3

```bash
aws s3 cp file.txt s3://my-bucket-name/
```

---

## 6. Download a File from S3

```bash
aws s3 cp s3://my-bucket-name/file.txt .
```

---

## 7. Synchronize Local Folder with S3

```bash
aws s3 sync ./website s3://my-bucket-name
```

---

## 8. List EC2 Instances

```bash
aws ec2 describe-instances
```

---

## 9. Start an EC2 Instance

```bash
aws ec2 start-instances --instance-ids i-1234567890abcdef0
```

---

## 10. Stop an EC2 Instance

```bash
aws ec2 stop-instances --instance-ids i-1234567890abcdef0
```

---

## 11. Reboot an EC2 Instance

```bash
aws ec2 reboot-instances --instance-ids i-1234567890abcdef0
```

---

## 12. Describe IAM Users

```bash
aws iam list-users
```

---

## 13. List Lambda Functions

```bash
aws lambda list-functions
```

---

## 14. List DynamoDB Tables

```bash
aws dynamodb list-tables
```

---

## 15. List CloudWatch Alarms

```bash
aws cloudwatch describe-alarms
```

---

## 16. List RDS Databases

```bash
aws rds describe-db-instances
```

---

## 17. List VPCs

```bash
aws ec2 describe-vpcs
```

---

## 18. List Security Groups

```bash
aws ec2 describe-security-groups
```

---

## 19. List Availability Zones

```bash
aws ec2 describe-availability-zones
```

---

## 20. Get AWS Caller Identity

Displays the currently authenticated AWS account.

```bash
aws sts get-caller-identity
```

---

# AWS CLI Cheat Sheet

| Command                               | Description               |
| ------------------------------------- | ------------------------- |
| `aws --version`                       | Check AWS CLI version     |
| `aws configure`                       | Configure AWS credentials |
| `aws s3 ls`                           | List S3 buckets           |
| `aws s3 mb`                           | Create S3 bucket          |
| `aws s3 cp`                           | Upload/Download files     |
| `aws s3 sync`                         | Synchronize folders       |
| `aws ec2 describe-instances`          | List EC2 instances        |
| `aws ec2 start-instances`             | Start EC2 instance        |
| `aws ec2 stop-instances`              | Stop EC2 instance         |
| `aws ec2 reboot-instances`            | Reboot EC2 instance       |
| `aws iam list-users`                  | List IAM users            |
| `aws lambda list-functions`           | List Lambda functions     |
| `aws dynamodb list-tables`            | List DynamoDB tables      |
| `aws cloudwatch describe-alarms`      | List CloudWatch alarms    |
| `aws rds describe-db-instances`       | List RDS instances        |
| `aws ec2 describe-vpcs`               | List VPCs                 |
| `aws ec2 describe-security-groups`    | List Security Groups      |
| `aws ec2 describe-availability-zones` | List Availability Zones   |
| `aws sts get-caller-identity`         | Show current AWS account  |
| `aws help`                            | Display AWS CLI help      |

---

# Best Practices

* Use IAM users and roles with the principle of least privilege.
* Configure named profiles for multiple AWS accounts.
* Never hardcode AWS credentials in your code.
* Enable MFA for production accounts.
* Use `aws help` to explore available commands and options.
* Regularly update AWS CLI to the latest version.

---

# Learning Outcomes

After completing this repository, you will be able to:

* Configure the AWS CLI.
* Manage Amazon S3 buckets and objects.
* Start, stop, and monitor EC2 instances.
* Work with IAM, Lambda, DynamoDB, and RDS.
* Inspect networking resources such as VPCs and Security Groups.
* Automate common AWS management tasks using the command line.

---

# Resources

* AWS CLI Documentation
  [https://docs.aws.amazon.com/cli/](https://docs.aws.amazon.com/cli/)

* AWS Documentation
  [https://docs.aws.amazon.com/](https://docs.aws.amazon.com/)

* AWS Free Tier
  [https://aws.amazon.com/free/](https://aws.amazon.com/free/)

---

# Contributing

Contributions are welcome!

1. Fork this repository.
2. Create a new branch.
3. Commit your changes.
4. Push the branch.
5. Open a Pull Request.

---

# License

This project is licensed under the **MIT License**.

---

# Author

**Your Name**

GitHub: https://github.com/Mannuru-Mahesh
