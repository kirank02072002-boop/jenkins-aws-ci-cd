# Jenkins CI/CD Pipeline on AWS EC2 🚀

This project demonstrates a complete CI/CD pipeline using **Jenkins**, **Docker**, and **AWS EC2**.  
Every code commit automatically triggers build and deployment without manual intervention.

---

## 🛠 Tech Stack
- AWS EC2 (Ubuntu)
- Jenkins (Dockerized)
- Docker
- GitHub Webhooks
- HTML Demo Application

---

## 📐 Architecture Flow

GitHub (Push)
   ↓  
GitHub Webhook  
   ↓  
Jenkins Pipeline  
   ↓  
Docker Build  
   ↓  
Docker Run on EC2  
   ↓  
Application Live 🚀

---

## ⚙️ Pipeline Stages

1. **Checkout Code**
2. **Build Docker Image**
3. **Stop Old Container**
4. **Run New Container**

---

## 🌐 Application URLs

- Jenkins Dashboard:
----
http://:8081
---
- Deployed Application:
----
http://:8081
---
## 🔁 Automation

- GitHub Webhook triggers Jenkins automatically
- No manual build or deployment needed
- Fully automated CI/CD pipeline

---

## 📦 How to Use

1. Push code to GitHub
2. Jenkins auto-triggers pipeline
3. Docker image builds
4. App redeploys automatically

---

## ✅ Outcome

- Zero-downtime deployment
- Fully automated DevOps workflow
- Real-world CI/CD implementation

---

## 👨‍💻 Author
Kiran
