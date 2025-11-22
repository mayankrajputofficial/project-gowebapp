# Go Web Application – DevOps Demo (Docker, Kubernetes, CI/CD)

This repository contains a simple Go web application that I use to demonstrate practical DevOps skills, including containerization with Docker, deployment on Kubernetes, and automation using CI/CD pipelines.

---

## 🚀 Features

- Go-based web application (simple HTTP server)
- Containerized using Docker (`Dockerfile`)
- Kubernetes-ready using:
  - Raw manifests in `k8s/manifests/`
  - Helm chart in `helm/gowebappchart/`
- CI/CD ready with GitHub Actions workflows in `.github/workflows/`
- Can be deployed to:
  - Local Kubernetes (Minikube / kind)
  - Any cloud Kubernetes cluster (e.g. AWS EKS)

---

## 🧰 Tech Stack

- **Language:** Go
- **DevOps / Infra:** Docker, Kubernetes, Helm, GitHub Actions
- **Platform:** Linux, Kubernetes
- **Other:** YAML, HTTP, Git

---

## 🏗 Architecture

High-level flow:

1. Code is pushed to this GitHub repository.
2. GitHub Actions can:
   - Run Go tests (`main_test.go`)
   - Build a Docker image from `Dockerfile`
   - Push the image to a container registry (e.g. Docker Hub)
3. Kubernetes manifests / Helm chart are applied to a cluster.
4. The application is exposed via a Service and can be accessed via browser or curl.


![Website](static/images/golang-website.png)


