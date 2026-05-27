# AWS Highly Available Multi-Tier Architecture via Terraform

This repository contains Terraform configurations to deploy a secure, highly available, multi-tier web application architecture on AWS.

## 🏗️ Architecture Overview
- **Custom VPC** with 2 Public Subnets and 2 Private Subnets across 2 Availability Zones.
- **Application Load Balancer (ALB)** in public subnets to distribute inbound HTTP traffic.
- **EC2 Web Servers** running Apache in private subnets for enhanced security.
- **NAT Gateway** allowing private instances to securely fetch software updates from the internet.

## 🚀 How to Run
1. Initialize Terraform: `terraform init`
2. View Deployment Plan: `terraform plan`
3. Deploy Infrastructure: `terraform apply --auto-approve`
4. Destroy Resources: `terraform destroy --auto-approve`