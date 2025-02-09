# Platform Engineer Assignment

## 1️⃣ Overview
This project sets up Minikube with:
- Two applications (`blue-app` and `green-app`).
- Nginx Ingress for traffic routing (75% to blue, 25% to green).

## 2️⃣ Prerequisites
- Minikube installed
- Kubectl installed

## 3️⃣ Steps to Run
### 🚀 Start Minikube
```sh
minikube start

### 🛠 Apply Kubernetes Manifests

**Apply the deployment:**
kubectl apply -f blue-app.yaml
kubectl apply -f green-app.yaml
kubectl apply -f ingress-main.yaml
kubectl apply -f ingress-canary.yaml
