🚀 DevOps Flask CI/CD Project
📌 Project Overview

This project demonstrates an end-to-end DevOps workflow for a containerized Python Flask application.
It covers CI/CD automation, Docker containerization, deployment, and monitoring using industry-standard tools.

The goal of this project is to automate the build, delivery, and observability of an application following DevOps best practices.

🎯 Purpose of the Project

Automate application build and delivery

Ensure consistency across environments using Docker

Reduce manual deployment errors

Enable monitoring and visibility into application health

Demonstrate real-world DevOps skills for interviews

🛠 Tech Stack

Language: Python (Flask)

CI/CD: GitHub Actions

Containerization: Docker, Docker Compose

Monitoring: Prometheus, Grafana

Version Control: Git & GitHub

OS: Linux (Ubuntu)

📂 Project Structure
devops-flask-app/
│
├── app/
│   ├── app.py
│   └── requirements.txt
│
├── .github/
│   └── workflows/
│       └── ci.yml
│
├── Dockerfile
├── docker-compose.yml
├── prometheus.yml
├── README.md
└── .gitignore

⚙️ Application Endpoints
Endpoint	Description
/	Main application endpoint
/health	Health check endpoint
/metrics	Prometheus metrics endpoint
🐳 Dockerization

The application is containerized using Docker to ensure portability and consistency.

Build Docker Image
docker build -t flask-devops-app .

Run Container
docker run -d -p 5000:5000 flask-devops-app

🔁 CI/CD Pipeline (GitHub Actions)
What happens on every git push:

Source code is pulled from GitHub

Docker image is built

Image is pushed to Docker Hub

This ensures continuous integration and faster delivery.

🚀 Deployment

The application is deployed using Docker Compose, which manages multiple services easily.

docker-compose up -d

📊 Monitoring & Observability

Prometheus scrapes application metrics

Grafana visualizes metrics such as:

Request count

Application uptime

Performance indicators

Access URLs

App: http://localhost:5000

Prometheus: http://localhost:9090

Grafana: http://localhost:3000

(Default Grafana login: admin / admin)

🔄 CI vs CD Explanation

CI (Implemented): Automatic build and image push on code change

CD (Optional): Can be added using SSH or Kubernetes for auto-deployment

This design keeps deployments safe and controlled.

🧠 Key DevOps Concepts Demonstrated

Continuous Integration (CI)

Docker container lifecycle

Infrastructure as Code

Monitoring and observability

Linux server deployment

DevOps best practices

⭐ Future Improvements

Add Kubernetes for orchestration

Add Terraform for infrastructure provisioning

Enable auto-deployment (CD)

Add alerting via Slack or Email

👨‍💻 Author

Vinay Mishra
Aspiring DevOps Engineer
