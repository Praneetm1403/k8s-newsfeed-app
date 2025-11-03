# 📰 Newsfeed App - Kubernetes Deployment

A simple Node.js application containerized with Docker and deployed to Kubernetes using Minikube.

## 🚀 Features
- Node.js Express backend (`index.js`)
- Dockerized using `Dockerfile`
- Kubernetes Deployment (`deployment.yaml`)
- Kubernetes Service (`service.yaml`)
- Accessible via NodePort through Minikube tunnel

## 🧠 Commands to Run Locally

### 1. Start Minikube
```bash
minikube start

minikube image build -t newsfeed-app .

kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

minikube service newsfeed-service

