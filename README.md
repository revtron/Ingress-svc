# Kubernetes Ingress Setup

This repository demonstrates how to set up and use **Kubernetes Ingress** to expose services within a cluster via a single entry point.

## 📘 What is Ingress?

Ingress is a Kubernetes API object that manages external access to services within a cluster, typically HTTP and HTTPS traffic. It allows you to:

- Use a **single IP/domain** to route to multiple services
- Define **URL-based routing** (e.g., `/api` → one service, `/web` → another)
- Add **TLS/SSL** termination
- Centralize **authentication, rate limiting**, and **logging**

---

## 🛠️ Components in This Setup

- **Nginx Ingress Controller** (installed via `minikube addons enable ingress`)
- **Ingress Object** (defines routing rules)
- **Two sample apps/services** (e.g., `web-service`, `api-service`)
- **Deployment files** for services and ingress

---

## 🚀 Quick Start (with Minikube)

1. **Start Minikube:**

   ```bash
   minikube start
