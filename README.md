# eks_project
eks resume project
# 🚀 CI/CD Pipeline for Kubernetes Deployment on AWS EKS

## 📌 Project Overview

This project demonstrates an end-to-end CI/CD pipeline that automates application build, testing, security scanning, containerization, and deployment to Kubernetes using AWS EKS. The pipeline ensures faster, reliable, and secure application delivery using DevOps best practices.

---

## ⚙️ Tech Stack

* **CI/CD Tool:** Jenkins
* **Source Control:** GitHub
* **Containerization:** Docker
* **Orchestration:** Kubernetes (EKS)
* **Cloud Platform:** AWS (ECR, EKS)
* **Code Quality:** SonarQube
* **Security Scanning:** Trivy
* **Monitoring:** CloudWatch, Prometheus

---

## 🔄 CI/CD Pipeline Flow

1. Developer pushes code to GitHub
2. Jenkins pipeline is triggered automatically
3. Application build and testing
4. Code quality analysis using SonarQube
5. Security scanning using Trivy
6. Docker image is built
7. Image is pushed to AWS ECR
8. Application is deployed to EKS using Kubernetes manifests
9. Rolling updates ensure zero downtime
10. Rollback strategy in case of failures

---

## 📁 Project Structure

```
ci-cd-eks-pipeline/
│── Jenkinsfile
│── Dockerfile
│── README.md
│── .gitignore
│── src/
│── k8s/
│    ├── deployment.yaml
│    └── service.yaml
│── docs/
```

---

## 🐳 Docker Build

```bash
docker build -t my-app .
docker run -p 3000:3000 my-app
```

---

## ☸️ Kubernetes Deployment

```bash
kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml
```

---

## 🔐 Secrets Management

* Jenkins credentials used for:

  * AWS authentication
  * SonarQube tokens

* Kubernetes secrets used for:

  * Database passwords
  * API keys

---

## 📈 Auto Scaling (HPA)

Horizontal Pod Autoscaler is used to automatically scale pods based on CPU usage, ensuring efficient resource utilization.

---

## 🔍 Monitoring

* **CloudWatch:** Infrastructure logs and metrics
* **Prometheus + Grafana:** Application-level monitoring

---

## ✅ Key Features

* Automated CI/CD pipeline using Jenkins
* Integrated code quality and security checks
* Docker-based containerization
* Kubernetes deployment on AWS EKS
* Rolling updates with zero downtime
* Rollback mechanism for failure recovery
* Multi-environment deployment support (Dev, Staging, Prod)

---

## 🧠 Learnings

* Hands-on experience with CI/CD pipeline design
* Understanding of Kubernetes deployments and scaling
* Implementation of DevSecOps practices
* AWS cloud deployment and container orchestration

---

## 📌 Future Improvements

* Helm charts for advanced deployments
* GitHub Actions integration
* Advanced monitoring dashboards
* Blue-Green / Canary deployments

---

## 👩‍💻 Author

**Shreyushi T R**

---

## ⭐ Conclusion

This project showcases a real-world CI/CD pipeline implementation using modern DevOps tools and practices, ensuring scalable, secure, and efficient application deployment.
