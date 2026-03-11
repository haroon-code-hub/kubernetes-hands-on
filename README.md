# Kubernetes Hands-On

A hands-on DevOps project that deploys a multi-service containerized application on Kubernetes using core Kubernetes resources such as Deployments, Services, ConfigMaps, and Persistent Volume Claims.

This project demonstrates practical Kubernetes fundamentals such as workload deployment, service exposure, configuration management, and rolling updates.

## Tech Stack

- Kubernetes
- Docker
- Minikube
- kubectl
- ConfigMaps
- Persistent Volume Claims

## Project Goals

- Deploy a multi-service containerized application on Kubernetes
- Manage container workloads using Kubernetes manifests
- Configure applications using ConfigMaps
- Persist data using PVCs
- Practice rolling updates and service management

## Architecture
User -> Service -> Web Pod -> API Pod -> Persistent Storage


## Kubernetes Resources Used

- Deployment
- Service
- ConfigMap
- PersistentVolumeClaim
- Rolling updates

## Repository Structure (sample)
├── api-deployment.yaml
├── api-service.yaml
├── web-deployment.yaml
├── web-service.yaml
├── configmap.yaml
├── pvc.yaml
└── README.md


## Prerequisites

Before running this project, install:

- Docker
- kubectl
- Minikube

## Getting Started

### Start the Kubernetes cluster
minikube start

### Apply the Kubernetes manifests
kubectl apply -f .


### Verify resources
kubectl get pods
kubectl get services
kubectl get pvc

### Access the application


minikube service <service-name>

## What I Practiced

- Deploying containerized applications on Kubernetes
- Managing services and workloads with kubectl
- Using ConfigMaps for environment configuration
- Persisting data with Persistent Volume Claims
- Performing rolling updates on deployments
