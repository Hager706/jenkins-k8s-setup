# 📌 Jenkins Kubernetes Setup  

This repository contains Kubernetes manifests to deploy **Jenkins** on **Minikube**.  

## 🔗 Related Repository  
For the Jenkins pipeline and Docker build, check:  
➡️ [Jenkins Docker Pipeline Lab](https://github.com/Hager706/jenkins-docker-pipeline-lab)  

---

## 🚀 Setup Steps  

### 1️⃣ Clone the Repository  
```sh
git clone https://github.com/Hager706/jenkins-k8s-setup.git
cd jenkins-k8s-setup
```

### 2️⃣ Start Minikube  
```sh
minikube start
```

### 3️⃣ Deploy Jenkins on Kubernetes  
```sh
kubectl apply -f jenkins-deployment.yml
kubectl apply -f jenkins-service.yml
```

### 4️⃣ Get Jenkins URL  
```sh
minikube service jenkins --url
```
Copy and open the **URL** in your browser to access Jenkins.  

---

## 📂 Repository Files  
- **`jenkins-deployment.yml`** → Deploys Jenkins as a pod.  
- **`jenkins-service.yml`** → Exposes Jenkins with a Kubernetes service.  

---
