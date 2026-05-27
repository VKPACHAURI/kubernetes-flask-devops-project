# 🚀 Flask Kubernetes Helm CI/CD Project

## 📌 Project Overview

This project demonstrates an end-to-end DevOps implementation using:

- Python Flask Application
- Docker Containerization
- Kubernetes Deployment
- Ingress Controller
- TLS/HTTPS Configuration
- Helm Charts
- Jenkins CI/CD Pipeline

The goal of this project is to simulate a real-world production deployment workflow using modern DevOps tools.

---

# 🛠️ Tools & Technologies Used

| Tool | Purpose |
|------|----------|
| Python Flask | Web Application |
| Docker | Containerization |
| Kubernetes | Container Orchestration |
| Helm | Kubernetes Package Management |
| Jenkins | CI/CD Automation |
| AWS EC2 | Cloud Infrastructure |
| Ingress NGINX | Routing & Load Balancing |

---

# 📂 Project Structure

```bash
flask-k8s-helm-cicd/
│
├── app.py
├── requirements.txt
├── Dockerfile
├── Jenkinsfile
│
├── kubernetes/
│   ├── deployment.yaml
│   ├── service.yaml
│   ├── ingress.yaml
│
├── flask-chart/
│   ├── Chart.yaml
│   ├── values.yaml
│   ├── values-dev.yaml
│   ├── values-stage.yaml
│   ├── values-prod.yaml
│   └── templates/
│
└── README.md
```

---

# 🐳 Docker Setup

## Build Docker Image

```bash
docker build -t flask-app:v1 .
```

## Run Container

```bash
docker run -d -p 5000:5000 flask-app:v1
```

---

# ☸️ Kubernetes Deployment

## Apply Deployment

```bash
kubectl apply -f deployment.yaml
```

## Apply Service

```bash
kubectl apply -f service.yaml
```

## Apply Ingress

```bash
kubectl apply -f ingress.yaml
```

---

# ⛵ Helm Chart Deployment

## Install Helm Chart

```bash
helm install myapp flask-chart/
```

## Upgrade Helm Chart

```bash
helm upgrade myapp flask-chart/
```

## Use Different Environments

### Dev Environment

```bash
helm install myapp flask-chart/ -f values-dev.yaml
```

### Stage Environment

```bash
helm install myapp flask-chart/ -f values-stage.yaml
```

### Production Environment

```bash
helm install myapp flask-chart/ -f values-prod.yaml
```

---

# 🔥 Jenkins CI/CD

Implemented Jenkins pipeline for:

- GitHub Integration
- Docker Build Automation
- CI/CD Workflow
- Kubernetes Deployment Automation

---

# 📖 Key Learnings

- Kubernetes Networking
- Helm Templating
- Multi-Environment Deployment
- Docker Containerization
- Jenkins Pipelines
- CI/CD Automation
- Kubernetes Troubleshooting

---

# 🚀 Future Enhancements

- DockerHub Push Automation
- Helm-based Auto Deployment
- ArgoCD GitOps
- Monitoring with Prometheus & Grafana
- Kubernetes Secrets Management

---

# 👨‍💻 Author

Vishesh Pachauri

---

# ⭐ If you like this project, give it a star!
