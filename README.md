# MEAN Stack DevOps Assignment

This project demonstrates containerization, CI/CD automation, and cloud deployment of a full-stack MEAN (MongoDB, Express, Angular, Node.js) application.

The application allows users to create, view, update, delete, and search tutorials.

---

## Tech Stack
- Angular
- Node.js & Express
- MongoDB
- Docker & Docker Compose
- GitHub Actions
- AWS EC2 (Ubuntu)
- Nginx

---

## Architecture
GitHub → GitHub Actions → Docker Hub → AWS EC2 → Docker Compose → Nginx → Application

---

## Prerequisites
- AWS EC2 Ubuntu instance
- Docker & Docker Compose installed
- Git installed
- Docker Hub account

---

## Deployment Steps

Clone Repository
git clone https://github.com/harshraisaxena/DevOps-Task.git
cd DevOps-Task

Run Application
docker-compose pull
docker-compose up -d

Open in browser
http://<EC2_PUBLIC_IP>

---

## Docker Images
harshraisaxena/mean-backend  
harshraisaxena/mean-frontend  

---

## CI/CD Pipeline
On every push to the main branch:
- Builds backend and frontend Docker images
- Pushes images to Docker Hub using GitHub Actions

---

## Nginx Reverse Proxy
- Port 80 → Frontend  
- /api → Backend  

---

## Screenshots

GitHub Actions Success  
screenshots/actions-success.png

Docker Hub Images  
screenshots/dockerhub-images.png

Application Running  
screenshots/app-running.png

Nginx Configuration  
screenshots/nginx-config.png

---

## Author
Harsh Rai Saxena
