📌 Trend Application – DevOps CI/CD Capstone Project
🚀 Project Overview

This project demonstrates a complete production-style DevOps workflow for deploying a React application using:

Infrastructure as Code (Terraform)

Containerization (Docker)

CI/CD automation with Jenkins

Kubernetes orchestration on Amazon Web Services

Monitoring using Prometheus and Grafana

Source control using GitHub

🧱 Tech Stack
Layer	Tools
Version Control	GitHub
Infrastructure	Terraform, AWS
CI/CD	Jenkins
Container	Docker, DockerHub
Orchestration	Kubernetes (EKS)
Monitoring	Prometheus, Grafana
☁ Infrastructure Provisioning (Terraform)

Terraform is used to provision:

VPC & Subnet

Security Group

EC2 instance for Jenkins

Terraform Workflow
terraform init
terraform plan
terraform apply


This automatically creates cloud infrastructure instead of manual provisioning.

⚙ Jenkins CI/CD Pipeline Flow

Code pushed to GitHub

Jenkins triggered automatically via webhook

Docker image built

Image pushed to DockerHub

Kubernetes deployment updated on AWS EKS

Pipeline is fully automated on every commit.
🐳 Docker

Application containerized using Dockerfile

Production build served via Nginx

Jenkins handles automated image creation and push

☸ Kubernetes (AWS EKS)

Resources used:

deployment.yaml → application pods

service.yaml → LoadBalancer exposure

Application is publicly accessible using AWS LoadBalancer.

📊 Monitoring

Monitoring stack includes:

Prometheus for metrics collection

Grafana for visualization

PVC storage managed using AWS EBS CSI driver.

🌐 Live Application

Application is exposed using Kubernetes LoadBalancer service on AWS.

📸 Screenshots Included

Jenkins pipeline successful execution

DockerHub image repository

Kubernetes pods & services

Grafana monitoring dashboard

Live application in browser

📁 Project Structure
Trend/
 ├── Dockerfile
 ├── Jenkinsfile
 ├── deployment.yaml
 ├── service.yaml
 ├── dist/
 ├── README.md

terraform/
 └── main.tf

✅ Key Achievements

✔ Infrastructure automated using Terraform
✔ End-to-end CI/CD pipeline
✔ Auto deployment on Kubernetes
✔ Monitoring enabled
✔ Cloud production workflow

🏁 Conclusion

This project implements a complete DevOps lifecycle from infrastructure provisioning to automated application deployment and monitoring in a cloud-native environment.

📌 Tools Used

Terraform | AWS | Docker | Jenkins | Kubernetes | Prometheus | Grafana | GitHub

🎯 Author

Capstone Project – DevOps Engineering
