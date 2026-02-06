Trend Application – DevOps CI/CD Deployment
Project Overview

React application deployed in a production-ready cloud environment using Docker, Kubernetes, Jenkins CI/CD and monitoring.

Tech Stack

GitHub for version control

Docker & DockerHub

Jenkins CI/CD

AWS EKS (Kubernetes)

Prometheus & Grafana

Infrastructure

AWS EC2 for Jenkins

AWS EKS cluster for application

LoadBalancer service for public access

CI/CD Pipeline Flow

Code pushed to GitHub

Jenkins builds Docker image

Image pushed to DockerHub

Kubernetes deployment updated automatically

Webhook triggers pipeline on every commit.

Kubernetes

deployment.yaml for pods

service.yaml for LoadBalancer exposure

Monitoring

Prometheus metrics

Grafana dashboards

Screenshots Included

Jenkins pipeline success

DockerHub image

Kubernetes pods & service

Grafana dashboard

Live application
