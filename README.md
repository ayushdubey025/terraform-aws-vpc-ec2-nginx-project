# AWS Infrastructure Automation using Terraform

## 🚀 Project Overview

This project automates the deployment of AWS infrastructure using Terraform, including:

- Custom VPC creation
- Public Subnet provisioning
- Internet Gateway and Route Table setup
- Security Group configuration (SSH + HTTP access)
- EC2 instance deployment with automated NGINX web server installation via User Data
- Modularized reusable Terraform code structure
- Parameterized variables and outputs for flexibility

## 🗺 Architecture Diagram

Internet ➔ Internet Gateway ➔ Public Subnet ➔ EC2 (NGINX) ➔ Security Groups

## 🧰 Technologies Used

- AWS (EC2, VPC, Subnet, Security Groups, IGW, Route Table)
- Terraform (Infrastructure as Code)
- NGINX (Web Server)
- Linux (Amazon Linux 2023)
- GitHub (Version Control)

## 📸 Screenshots

### Terraform Init

![Terraform Init](screenshots/terraform-init.png)

### Terraform Plan

![Terraform Plan](screenshots/terraform-plan1.png)
![Terraform Plan](screenshots/terraform-plan2.png)

### Terraform Apply

![Terraform Apply](screenshots/terraform-apply.png)

### AWS VPC Console

![AWS VPC](screenshots/vpc-created.png)

### AWS Subnet Console

![AWS Subnet](screenshots/subnet-created.png)

### AWS EC2 Console

![AWS EC2](screenshots/ec2-created.png)

### NGINX Web Page (Browser Output)

![NGINX](screenshots/nginx-web.png)

### Terraform Destroy

![Terraform Destroy](screenshots/terraform-destroy.png)

## ⚙ How to Run This Project

1. Clone the repository.
2. Configure your AWS CLI credentials.
3. Create an AWS Key Pair for SSH access.
4. Edit `terraform.tfvars` with your key name.
5. Initialize Terraform:

```bash
terraform init
