# Trend Application DevOps Deployment

## Project Overview
This project demonstrates a complete CI/CD pipeline using Jenkins, Docker, and Kubernetes (AWS EKS).

## Architecture
GitHub → Jenkins → Docker Build → DockerHub → Kubernetes Deploy → LoadBalancer

## Tools Used
- AWS EC2
- Jenkins
- Docker
- DockerHub
- Amazon EKS
- Kubernetes
- GitHub

## Setup Steps

1. Created AWS EC2 instance
2. Installed Docker, kubectl, eksctl
3. Created EKS cluster
4. Dockerized React application
5. Pushed image to DockerHub
6. Created Kubernetes deployment and service
7. Installed Jenkins and configured pipeline
8. Automated build and deploy using GitHub webhook

## Pipeline Stages
- Checkout Code
- Build Docker Image
- Push to DockerHub
- Deploy to Kubernetes

## Application Access (Kubernetes LoadBalancer)
The application is deployed on AWS EKS using Kubernetes LoadBalancer.
**LoadBalancer URL:**
  http://ac98f0b6d39f54337af69e4c074065b7-1492213178.ap-south-1.elb.amazonaws.com
Open this URL in browser to access the application.

## Output
Application deployed successfully using Kubernetes LoadBalancer.

## Screenshots
(Add Jenkins pipeline success, EKS nodes, LoadBalancer output)
