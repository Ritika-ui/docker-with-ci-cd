# 🚀 Dockerized Web App with CI/CD Pipeline

## 📌 Overview

This project demonstrates a complete DevOps workflow:

* Containerized backend application using Docker
* Reverse proxy setup using Nginx
* Automated CI pipeline using GitHub Actions
* Docker image build and push to Docker Hub

---

## 🧱 Tech Stack

* Docker 🐳
* Nginx 🌐
* GitHub Actions ⚙️
* Backend (Flask / Node — update this)

---

## 🔁 Project Flow

Browser → Nginx → Backend (Port 5000)

CI Flow:
Push Code → GitHub Actions → Build Docker Image → Push to Docker Hub

---

## 🐳 Docker Setup

### Build image

docker build -t your-dockerhub-username/myapp .

### Run container

docker run -p 5000:5000 your-dockerhub-username/myapp

---

## ⚙️ CI/CD Pipeline

* On every push to `main`:

  * Code is checked out
  * Docker image is built
  * Image is pushed to Docker Hub

---

## 📦 Docker Hub Repository

your-dockerhub-username/myapp

---

## 🌐 Nginx Reverse Proxy

Nginx acts as a mediator:

* Receives request from browser
* Forwards to backend container
* Returns response

---

## 🚀 Future Improvements

* Add CD (deployment to cloud)
* Use HTTPS
* Add database support

---

## 👩‍💻 Author

Ritika Khadka
