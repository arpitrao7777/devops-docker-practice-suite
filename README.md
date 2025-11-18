# devops-docker-practice-suite

This repository contains a collection of Dockerfiles for practicing containerization with different technologies, including a **.NET backend**, a **Node.js frontend**, and a **multi-stage Docker build** workflow using **Nginx**.  
The goal of this project is to help understand how Docker builds, copies artifacts, uses multi-stage images, and optimizes lightweight production-ready containers.

---

## **🚀 What This Repository Covers**

- **Multi-stage build for .NET backend**  
- **Node.js frontend build** served using **Nginx**
- **Optimized multi-stage Docker images**
- Understanding how to use:  
  - `COPY --from=build`  
  - layered caching  
  - artifact copying  
- **Reducing image size** and improving build performance

---

## **🧩 How to Build & Run**

### **Backend (.NET)**
```bash
cd backend
docker build -t backend-app.
docker run -p 5000:80 backend-app
```

Frontend (Node → Nginx)
```bash
cd frontend
docker build -t frontend-app.
docker run -p 8080:80 frontend-app
```
Multi-Stage Frontend Build
```bash
cd multi_stage_dockerfile
docker build -t frontend-multistage.
docker run -p 8081:80 frontend-multistage
```

**🛠️ Technologies Used**
Docker

.NET 8 SDK & Runtime

Node.js

NPM

Nginx

Multi-stage Docker builds

**📚 Purpose of This Repo**
This repository is created to:

Practice Docker fundamentals

Understand backend + frontend containerization

Learn multi-stage image optimization

Prepare for DevOps, Docker, and Kubernetes workflows

Improve hands-on experience with real-world Dockerfile structures

**📬 Contact**
Arpit Yadav
📱 8307532971
✉️ arpit32971@gmail.com

LinkedIn: https://www.linkedin.com/in/arpit-yadav-786b1622b
