# Trend Application DevOps Deployment

## Project Overview

This project demonstrates a complete end-to-end DevOps CI/CD pipeline using Jenkins, Docker, Kubernetes (AWS EKS), Infrastructure as Code using Terraform, and monitoring using Prometheus and Grafana.

The application is containerized using Docker, deployed to AWS EKS through Jenkins CI/CD pipeline, infrastructure provisioned using Terraform, and monitored using Prometheus and Grafana.

---

## Architecture

GitHub → Jenkins → Docker Build → DockerHub → Kubernetes (AWS EKS) → LoadBalancer → Monitoring (Prometheus + Grafana)

---

## Tools Used

* AWS EC2
* Terraform (Infrastructure as Code)
* Jenkins
* Docker
* DockerHub
* Amazon EKS
* Kubernetes
* Prometheus
* Grafana
* Node Exporter
* GitHub

---

## Infrastructure Setup (Terraform)

Infrastructure was provisioned using Terraform:

* Created EC2 instance using Terraform
* Created Security Group using Terraform
* Installed Jenkins on Terraform provisioned instance
* Infrastructure deployed using:

  * terraform init
  * terraform plan
  * terraform apply

---

## Setup Steps

* Created AWS infrastructure using Terraform
* Installed Docker, kubectl, eksctl
* Created AWS EKS cluster
* Dockerized React application
* Pushed Docker image to DockerHub
* Created Kubernetes deployment and service
* Installed Jenkins and configured pipeline
* Automated build and deploy using GitHub webhook
* Configured monitoring using Prometheus and Grafana

---

## Pipeline Stages (Jenkins CI/CD)

* Checkout Code from GitHub
* Build Docker Image
* Push Docker Image to DockerHub
* Deploy Application to Kubernetes (EKS)

---

## Kubernetes Deployment

* EKS cluster created
* Node group configured
* Kubernetes deployment.yaml and service.yaml created
* Application exposed using LoadBalancer service
* Application accessed via external URL

---

## Monitoring Setup

* Prometheus installed for metrics collection
* Node Exporter configured to collect system metrics
* Prometheus targets configured and running
* Grafana installed for visualization
* Monitoring dashboard created using Grafana

---

## Application Access (Kubernetes LoadBalancer)

The application is deployed on AWS EKS using Kubernetes LoadBalancer.

LoadBalancer URL:
http://ac98f0b6d39f54337af69e4c074065b7-1492213178.ap-south-1.elb.amazonaws.com

Open this URL in browser to access the application.

---

## Output

* Infrastructure provisioned using Terraform
* CI/CD pipeline automated using Jenkins
* Application deployed successfully to AWS EKS
* Monitoring enabled using Prometheus and Grafana
* Application accessible via LoadBalancer

---

## Screenshots

* Terraform execution
* Jenkins pipeline success
* Docker image push
* EKS nodes and pods
* Kubernetes LoadBalancer output
* Application running
* Prometheus targets
* Grafana dashboard
