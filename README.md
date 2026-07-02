# 🚀 Django Production Deployment on AWS using CloudFormation

This project demonstrates a **production-grade AWS infrastructure** for deploying a Django web application using **AWS CloudFormation (Infrastructure as Code)**.

It follows a **modular nested stack architecture** with separation of concerns for scalability, security, and maintainability.

---

## 🏗️ Architecture Overview

The infrastructure is divided into 4 main stacks:

### 1. Network Stack
- VPC creation
- Public and private subnets
- Internet Gateway & routing

### 2. Security Stack
- Security Groups (ALB, EC2, RDS)
- IAM Role for EC2 instance
- Instance Profile configuration

### 3. Compute Stack
- EC2 Launch Template
- Auto Scaling Group (ASG)
- Application Load Balancer (ALB)
- Target Group + Listener
- Django deployment using Gunicorn + Nginx

### 4. Database Stack
- Amazon RDS MySQL instance
- DB Subnet Group
- Parameter Group
- Automated backups
- Secure private database access

---

## 📂 Project Structure
