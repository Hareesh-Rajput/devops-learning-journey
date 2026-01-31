🔗 Setup screenshots are available on my <a href="YOUR_LINKEDIN_POST_URL" target="_blank">
<img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" width="16"/> LinkedIn post
</a>

# GitLab CI/CD Setup using Docker Compose

This repository contains a complete setup of a **self-hosted GitLab Server** and a **GitLab Runner**
using **Docker Compose**.  
The setup is suitable for learning, practicing DevOps concepts, and running CI/CD pipelines locally.

---

## 🚀 Features

- GitLab Server running in Docker
- GitLab Runner with Docker executor
- Persistent data using Docker volumes
- CI/CD ready environment
- Easy start/stop using Docker Compose
- Beginner & interview friendly setup

---

## 🧱 Architecture Overview

Developer → GitLab Server → GitLab Runner → CI/CD Jobs


- **GitLab Server** manages repositories, users, and pipelines
- **GitLab Runner** executes CI/CD jobs defined in `.gitlab-ci.yml`

---


---

## ⚙️ Prerequisites

Make sure you have the following installed:

- Docker
- Docker Compose
- Git
- Minimum 4 GB RAM (GitLab is resource intensive)

---

## ▶️ Setup & Run

### 1️⃣ Clone the repository
```bash
git clone https://github.com/<your-username>/gitlab-ci-cd-docker-compose.git
cd gitlab-ci-cd-docker-compose

2️⃣ Start GitLab Server & Runner

docker compose up -d

⏳ First startup may take 10–15 minutes

3️⃣ Access GitLab

http://localhost:8000

Login credentials

Username: root

Password: *****
(For learning purposes only)

🔧 GitLab Runner Setup

The GitLab Runner is configured using Docker executor.

Verify runner inside container

docker exec -it my-gitlab-runner gitlab-runner list

Expected output:
Executor=docker
URL=http://my-gitlab-server



