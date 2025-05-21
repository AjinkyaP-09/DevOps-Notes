# 🌐 Terraform Overview + EC2 Deployment on AWS (Mumbai)

This repository provides a basic understanding of **Terraform** along with a hands-on practical to launch an **AWS EC2 instance** in the **ap-south-1 (Mumbai)** region.

## 📘 Overview

- Introduction to Terraform and its components: **providers, resources, modules, variables, state files, and outputs**
- How Terraform interacts with **AWS** using secure access credentials
- Steps to configure and launch an EC2 instance using Terraform
- Generating and managing SSH key pairs within Terraform
- Outputting instance details like **public IP** and **instance ID**
- Clean-up using `terraform destroy`

## 🧪 Technologies Used

- Terraform
- AWS (EC2, Key Pair)
- VS Code (optional)
- Linux Shell / Terminal

## 📁 Project Files

- `main.tf` – Main configuration with provider, EC2 resource, key pair
- `variables.tf` – Input variable definitions
- `terraform.tfvars` – Values for region, AMI, and instance type
- `outputs.tf` – Outputs: instance public IP, ID, and SSH user

## ✅ How to Run

1. Set AWS credentials in environment variables
2. Run `terraform init` → `terraform plan` → `terraform apply`
3. Get SSH access to your instance using the auto-generated key
4. Destroy the setup with `terraform destroy`

## 🔒 Security Note

- Key pairs are **generated programmatically**
- Private key is **saved locally** and **not reused**
- Credentials are **not hardcoded**

### Document: [Terraform-1.docx](./Terraform-1.docx)

---

**Author**: Ajinkya Pame  
🔗 [LinkedIn](https://www.linkedin.com/in/ajinkya-pame-4a752b346)
