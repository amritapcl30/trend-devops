# CI/CD Deployment of React Application on AWS EKS

## 📌 Project Overview
This project demonstrates an end-to-end CI/CD pipeline for deploying a React frontend application on AWS using Docker, Jenkins, Terraform, and Kubernetes (EKS). The pipeline automates application build, containerization, deployment, and public exposure via a Kubernetes LoadBalancer.

---

## 🛠 Tools & Technologies

- Docker
- Jenkins
- Terraform
- AWS (EC2, EKS)
- DockerHub
- Kubernetes
- Kubernetes Metrics Server (Open Source Monitoring)

---

## 🏗 Architecture Summary
- Source code is hosted on GitHub
- Jenkins (running on EC2) builds and pushes Docker images to DockerHub
- Application is deployed to AWS EKS using Kubernetes manifests
- Kubernetes LoadBalancer exposes the application publicly

---

## 🧱 Infrastructure Provisioning
Terraform is used to provision AWS infrastructure including:
- VPC
- Security Groups
- EC2 instance for Jenkins

### Terraform Commands
```bash
terraform init
terraform plan
terraform apply
