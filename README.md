# 🚀 Infrastructure Automation using Terraform on AWS

## 📌 Project Overview

This project demonstrates **Infrastructure as Code (IaC)** by automating AWS infrastructure provisioning using **Terraform**. The goal is to create, manage, and destroy cloud resources in a **reliable, repeatable, and automated way** without manual intervention.

This project provisions an **EC2 instance on AWS** using Terraform scripts, following DevOps best practices for automation and version control.

---

## 🎯 Project Objectives

* Automate AWS infrastructure provisioning using Terraform.
* Implement Infrastructure as Code (IaC) practices.
* Create reusable and modular Terraform configuration files.
* Reduce manual configuration errors.
* Improve infrastructure deployment speed and reliability.

---

## 🛠️ Tech Stack & Tools

* **Cloud Platform:** AWS (EC2, Security Group)
* **Infrastructure as Code Tool:** Terraform
* **Version Control:** Git & GitHub
* **Operating System:** Linux

---

## 🏗️ Project Architecture

```
User → Terraform → AWS Provider → EC2 Instance Deployment
```

### Flow Explanation:

1. User executes Terraform commands.
2. Terraform reads configuration files.
3. AWS resources are automatically created.
4. Output displays public IP of deployed EC2 instance.

---

## 📂 Project Folder Structure

```
terraform-aws-infra
│
├── main.tf
├── provider.tf
├── variables.tf
├── outputs.tf
└── README.md
```

---

## ⚙️ Terraform Configuration Files Description

* **provider.tf** → Defines AWS provider and region.
* **main.tf** → Contains EC2 instance resource configuration.
* **variables.tf** → Stores reusable variable definitions.
* **outputs.tf** → Displays useful outputs like public IP.

---

## 🚀 How to Execute the Project

### Step 1: Install Terraform

```bash
sudo yum install -y yum-utils
sudo yum-config-manager --add-repo https://rpm.releases.hashicorp.com/AmazonLinux/hashicorp.repo
sudo yum -y install terraform
```

Verify installation:

```bash
terraform -version
```

---

### Step 2: Configure AWS Credentials

```bash
aws configure
```

Provide:

* AWS Access Key
* AWS Secret Key
* Region: ap-south-1
* Output format: json

---

### Step 3: Initialize Terraform

```bash
terraform init
```

---

### Step 4: Validate & Plan Infrastructure

```bash
terraform validate
terraform plan
```

---

### Step 5: Apply Configuration

```bash
terraform apply
```

Type **yes** when prompted.

---

### Step 6: Verify Deployment

* Login to AWS Console
* Navigate to EC2 Dashboard
* Verify EC2 instance is running

---

### Step 7: Destroy Infrastructure (Cleanup)

```bash
terraform destroy
```

---

## 🚀 Key Learnings

* Infrastructure provisioning using Terraform
* AWS resource automation
* Infrastructure as Code (IaC) implementation
* Real-world DevOps automation workflow

---

## 📈 Future Enhancements

* Add VPC and Subnet automation
* Create reusable Terraform modules
* Integrate Terraform with Jenkins CI/CD
* Automate multi-environment deployments (dev, staging, prod)

---

## 👨‍💻 Author

**Prathamesh Santosh Mahajan**
B.Tech Computer Engineering | DevOps & AWS Enthusiast

🔗 GitHub: [https://github.com/Prathamesh1305](https://github.com/Prathamesh1305)

---

⭐ If you find this project useful, don't forget to **star the repository**!
