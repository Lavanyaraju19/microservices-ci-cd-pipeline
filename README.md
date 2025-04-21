
# 🚀 Microservices CI/CD Pipeline with Jenkins & Docker

This project demonstrates a production-style **CI/CD pipeline** to automate build, test, and deployment for a **Node.js microservice** using **Jenkins** and **Docker**.

The goal is to simulate real-world continuous delivery using containerization, pipeline-as-code (Jenkinsfile), and automated testing, following DevOps best practices.

---

## ⚙️ Tech Stack

- **Jenkins** – CI/CD server
- **Docker** – Containerization
- **Node.js** – Microservice backend
- **Shell Scripting** – Deployment automation
- **Jenkinsfile** – Pipeline as Code

---

## 🗂️ Project Structure

```plaintext
microservices-ci-cd-pipeline/
├── Jenkinsfile                # CI/CD pipeline definition
├── backend/                   # Microservice source code
│   ├── Dockerfile             # Builds Docker image for Node.js app
│   ├── server.js              # Simple backend API
│   ├── test_backend.py        # Basic test script
│   ├── package.json           # Node dependencies
│   └── node_modules/          # Local dependencies
└── README.md                  # Project documentation

🚀 Pipeline Workflow (Jenkinsfile)
Clone Source Code

Install Dependencies

Run Tests

Build Docker Image

Push to DockerHub (optional)

Deploy to Container Runtime
✅ Prerequisites
Jenkins installed locally or on cloud (e.g., Jenkins on EC2 or Docker)

Docker installed on Jenkins agent

GitHub repo connected to Jenkins job

Optional: DockerHub account for pushing images

🧪 Running the Pipeline
1️⃣ Set up Jenkins Job
Choose "Pipeline" project

Connect your GitHub repo

Paste contents of Jenkinsfile in pipeline config

2️⃣ Trigger the Pipeline
On push, Jenkins will:

Pull the code

Run tests via test_backend.py

Build Docker image

Tag and deploy (optional: push to DockerHub)

📦 Docker Commands (Manual Run Option)
bash
Copy
Edit
cd backend
docker build -t microservice-demo .
docker run -p 3000:3000 microservice-demo
📷 Optional Additions
Add test report publishing in Jenkins

Integrate with SonarQube or Nexus

Push to DockerHub

Deploy to Kubernetes or ECS

📜 License
MIT — use this project freely for learning and deployment demos.

✍️ Author
Lavanya J
DevOps Engineer
GitHub | LinkedIn
