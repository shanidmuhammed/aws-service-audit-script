# AWS Resource Listing Script

A Bash script to automate the process of listing various AWS resources within a specific region using the AWS CLI.

## 📌 Author

**Shanid V V**  
Version: `v0.0.1`

## 🧾 Description

This script allows you to quickly view details of AWS services in your account. It supports a variety of AWS services and can be executed from any environment where the AWS CLI is installed and configured.

### ✅ Supported AWS Services:
- EC2
- S3
- RDS
- DynamoDB
- Lambda
- EBS
- ELB
- CloudFront
- CloudWatch
- SNS
- SQS
- Route53
- VPC
- CloudFormation
- IAM

## ⚙️ Prerequisites

- **AWS CLI** must be installed.
- **AWS credentials** must be configured using `aws configure`.

##  Usage:
````bash
./aws_resources_list.sh <region> <service_name>
````
##  Example:
````bash
./aws_resources_list.sh us-east-1 ec2
````
This command lists all EC2 instances in the us-east-1 region.

## 📂 How It Works
- The script checks for valid input arguments.
- Verifies that AWS CLI is installed and configured.
- Matches the service name and runs the appropriate AWS CLI command for that service.

## 🛠️ Example Output:
````
Listing EC2 Instances in us-east-1
{
    "Reservations": [
        {
            "Instances": [
                {
                    "InstanceId": "i-0123456789abcdef0",
                    ...
                }
            ]
        }
    ]
}

````
