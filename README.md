# 🚀 DevOps Internship Assessment

## 📘 Overview
This project is created as part of the **DevOps Internship Assessment**.  
It demonstrates the ability to:

- Containerize a **Next.js** application using **Docker**
- Automate builds and push images to **GitHub Container Registry (GHCR)** using **GitHub Actions**
- Deploy the containerized application to **Kubernetes (Minikube)**

---

## 🧰 Tech Stack
- **Framework:** Next.js (Node.js 18)
- **Containerization:** Docker
- **CI/CD Automation:** GitHub Actions
- **Registry:** GitHub Container Registry (GHCR)
- **Orchestration:** Kubernetes (Minikube)
- **OS Used:** Ubuntu 22.04 LT


##  Project setup 
## Step 1: Clone the Repository
   git clone https://github.com/vaibhav7616/devops-intern-assessment.git
   cd devops-intern-assessment

## Step 2: Install Dependencies
   npm install

## Step 3: Run Locally
npm run dev

Visit: http://localhost:3000

##  Docker Setup (Local)
##  Build Docker Image
    docker build -t ghcr.io/vaibhav7616/devops-intern-assessment:latest .

## Run Container
  docker run -p 3000:3000 ghcr.io/vaibhav7616/devops-intern-assessment:latest


Test it at: http://localhost:3000

## GitHub Actions Workflow (CI/CD)

File Path: .github/workflows/ci-cd.yml
## GHCR Image
ghcr.io/vaibhav7616/devops-intern-assessment:latest

## Kubernetes Deployment (Minikube)
   Deployment Files
   Inside the k8s/ 

   
## Apply to Minikube
   kubectl apply -f k8s/deployment.yaml
   kubectl apply -f k8s/service.yaml

## Verify
   kubectl get pods
   kubectl get svc

## Access App
  minikube service nextjs-service --url

