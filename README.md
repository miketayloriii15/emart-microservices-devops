# 🛒 EMart Microservices DevOps Project

A microservices-based e-commerce application demonstrating DevOps practices and containerized deployment.

## 🚀 Architecture

- **Client (Front End):** Angular
- **API Gateway:** NGINX (routes requests to backend services)
- **EMart API:** Node.js + MongoDB
- **Books API:** Java + MySQL
- **Infrastructure:** Docker, Docker Compose, Vagrant (VM provisioning)
- **CI/CD:** Jenkins pipeline
- **Configuration:** `Vagrantfile`, `docker-compose.yaml`

markdown
Copy code
                     ┌─────────────┐
                     │   Angular   │
                     └──────┬──────┘
                            │
                    ┌───────▼────────┐
                    │    NGINX       │
                    └───┬────────────┘
            ┌───────────┴───────────┐
            │                       │
     ┌──────▼──────┐         ┌──────▼──────┐
     │ EMart API   │         │ Books API   │
     │ Node.js     │         │ Java        │
     │ MongoDB     │         │ MySQL       │
     └─────────────┘         └─────────────┘
bash
Copy code

## 🧩 Features
- User-facing Angular front end served via NGINX API gateway
- Node.js service for product & cart management (MongoDB backend)
- Java service for books management (MySQL backend)
- Fully containerized with Docker
- Orchestrated using docker-compose
- Vagrant provisioning for consistent development VM
- CI/CD pipeline example with Jenkins

## ⚡ Quick Start

```bash
# Clone the repository
git clone https://github.com/<your-username>/emart-microservices-devops.git
cd emart-microservices-devops

# Bring up Vagrant VM (if needed)
vagrant up

# Build & start containers
docker-compose up --build
Access the app in your browser at: http://192.168.56.82:80 (adjust IP if different in your Vagrantfile).

🛠️ Tech Stack
Frontend: Angular

Backend APIs: Node.js (MongoDB), Java Spring Boot (MySQL)

Gateway: NGINX

DevOps Tools: Docker, Docker Compose, Jenkins, Vagrant, VirtualBox

Databases: MongoDB, MySQL

📚 Learning Objectives
Microservices architecture with multiple languages

Containerization & multi-service orchestration

CI/CD pipeline with Jenkins

Provisioning Dev environments with Vagrant

👤 Author
Mike Taylor III — LinkedIn | GitHub

⚖️ License
MIT (or whatever license you choose)

yaml
Copy code

---

### ✅ Next steps
1. Initialize the repo:
```bash
cd containerIntro
git init
git add .
git commit -m "Initial commit: EMart microservices DevOps project"
git branch -M main
git remote add origin https://github.com/<your-username>/emart-microservices-devops.git
git push -u origin main
