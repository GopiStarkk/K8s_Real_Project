# Node.js Microservice CI/CD on Amazon EKS

## Overview

This project demonstrates a complete DevOps implementation for deploying a Node.js application to Amazon EKS using a fully automated CI/CD pipeline.

The solution integrates GitHub, Jenkins, SonarQube, Docker, Amazon ECR, Helm, Kubernetes, and NGINX Ingress Controller to automate application delivery from source code to production-ready Kubernetes workloads.

---

## Features

- Node.js application
- Dockerized application
- Amazon ECR integration
- Amazon EKS deployment
- Helm Charts
- Jenkins CI/CD
- SonarQube Static Code Analysis
- Kubernetes Secrets
- NGINX Ingress
- Automatic version tagging
- Zero manual deployment

---

## Technology Stack

- AWS EKS
- Terraform
- Jenkins
- GitHub
- Docker
- Amazon ECR
- Helm
- Kubernetes
- SonarQube
- NGINX Ingress

---

## Repository Structure

```text
src/
Dockerfile
Helm/
Jenkinsfile
docs/
README.md
```

---

## CI/CD Workflow

```
GitHub
   │
   ▼
Jenkins

SCM Checkout

SonarQube Scan

npm install

Docker Build

Push Image to Amazon ECR

Update kubeconfig

Helm Deployment

Verify Kubernetes Resources
```

---

## Result

Every Git commit automatically deploys the latest application version into Amazon EKS.
