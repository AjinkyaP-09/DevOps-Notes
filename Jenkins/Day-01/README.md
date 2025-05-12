# ✅ Jenkins Learning Journey - Day 1: Jenkins Fundamentals

## 🎯 Objectives Achieved

- Understood what Jenkins is and its role in CI/CD
- Set up Jenkins on an AWS EC2 Ubuntu instance
- Explored the Jenkins UI and core concepts
- Created and ran Freestyle and Pipeline jobs

---

## 🧠 Theory Summary

### 🔹 What is Jenkins?

Jenkins is an open-source automation server used to automate the building, testing, and deployment of software. It is a key component of Continuous Integration and Continuous Delivery (CI/CD) workflows.

- Open-source and widely adopted in DevOps
- Plugin-based architecture for extensibility
- Helps streamline software delivery pipelines

### 🔹 Jenkins Key Concepts

| Concept            | Description                                                                |
| ------------------ | -------------------------------------------------------------------------- |
| **Job**            | A task Jenkins performs (e.g., build, test, deploy)                        |
| **Freestyle Job**  | A simple job with shell steps or build scripts                             |
| **Pipeline**       | A job defined using a Jenkinsfile (code-based automation pipeline)         |
| **Plugins**        | Extend Jenkins functionality (e.g., Git, Docker, Slack integration)        |
| **Dashboard**      | Central interface to manage all jobs                                       |
| **Build Triggers** | Define how/when a job should be executed (manual, schedule, webhook, etc.) |

---

## 🛠️ Practical Tasks

### ✅ EC2 Setup

- Launched an Ubuntu EC2 instance on AWS
- Configured Security Group:
  - Port 22 (SSH)
  - Port 8080 (Jenkins Web UI)

### ✅ Jenkins Installation

- Installed **Java 17**
- Added Jenkins repository and GPG key
- Installed Jenkins using `apt`
- Enabled and started Jenkins service using `systemctl`

### ✅ Jenkins Access

- Accessed Jenkins via `http://<public-ip>:8080`
- Used initial admin password to unlock Jenkins
- Installed recommended plugins
- Created initial admin user account

### ✅ Created Jobs

- **Freestyle Job**: Ran a simple shell script
- **Pipeline Job**: Created a basic `Jenkinsfile` and executed it via the Pipeline project

---

📘 **Next Steps**: Dive deeper into Pipeline scripting, explore webhooks, and integrate GitHub repositories.
