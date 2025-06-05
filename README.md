# Kubernetes Minikube Deployment

## Objective
Deploy and manage applications locally using Kubernetes with Minikube.

## Tools Used
- Minikube
- kubectl
- Docker

## Steps Completed
1. Installed and started Minikube cluster locally on Amazon Linux EC2 instance.
2. Created a `deployment.yaml` file to deploy a sample Nginx application.
3. Created a `service.yaml` file to expose the application using NodePort.
4. Used `kubectl` commands to:
   - Deploy the app (`kubectl apply -f deployment.yaml`)
   - Expose the app (`kubectl apply -f service.yaml`)
   - Verify pods and services (`kubectl get pods`, `kubectl get svc`)
5. Scaled the deployment using `kubectl scale`.
6. Checked logs of pods with `kubectl logs`.

## Outcome
- Gained hands-on experience with Kubernetes basics: deployments, services, scaling, and pod logs.
- Understood how Minikube works to create a local Kubernetes environment.
- Learned to expose apps using NodePort for external access.

## How to Run
1. Start Minikube:  
   ```bash
   minikube start --driver=none

**Apply deployment and service YAMLs:**

kubectl apply -f deployment.yaml  
kubectl apply -f service.yaml

**Check pods and services:**
kubectl get pods  
kubectl get svc

**Scale deployment (example to 3 replicas):**
kubectl scale deployment nginx-deployment --replicas=3

**View logs:**
kubectl logs <pod-name>

