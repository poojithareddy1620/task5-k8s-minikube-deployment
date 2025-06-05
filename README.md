# Kubernetes Minikube Deployment - Task 5
**Access the App**

http://184.72.107.185:30080/

## Objective
Deploy and manage a sample Nginx application using Kubernetes on Minikube (Amazon Linux EC2 instance).

## Tools Used
- Minikube
- kubectl
- Docker
- Amazon Linux EC2

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/poojithareddy1620/task5-k8s-minikube-deployment.git
cd task5-k8s-minikube-deployment

**Apply Kubernetes YAML Files**

kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

**Verify Deployment and Service**
kubectl get pods
kubectl get svc


