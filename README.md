# 2048 Game Deployment on AWS EKS using Fargate

This project demonstrates how to deploy the 2048 web game on a Kubernetes cluster hosted on AWS EKS using Fargate for serverless compute. An AWS ALB Ingress Controller is configured to expose the application over the internet.

## Tech Stack Used:
- Amazon EKS (Fargate)
- Kubernetes
- AWS ALB Ingress Controller
- IAM, VPC, Subnets
- `eksctl`, `kubectl`, YAML
- AWS CloudWatch

## Project Structure
- `manifests/`: Kubernetes Deployment, Service, Ingress, and Namespace YAML files.
- `eksctl/`: EKS cluster and Fargate profile configs.
- `cleanup/`: Resource cleanup shell scripts.
- `screenshots/`: Proof of deployment.

## Setup Guide
1. Create your EKS cluster:
   bash
   eksctl create cluster -f eksctl/cluster-config.yaml
