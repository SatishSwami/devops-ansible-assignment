# DevOps Case Study & Ansible Automation

## 1. Project Title

**DevOps Automation of a Web Application using Ansible**

---

## 2. Problem Statement

Manual configuration and deployment of web servers can be time-consuming,
error-prone, and difficult to reproduce consistently.

This project demonstrates how DevOps practices and Ansible configuration
management can be used to automate the deployment and configuration of a
web application on an Ubuntu environment.

---

## 3. Objectives

The main objectives of this project are:

- Analyze a real-world web application DevOps lifecycle.
- Design a suitable DevOps architecture.
- Demonstrate configuration management using Ansible.
- Create an Ansible inventory for managing the target environment.
- Develop an Ansible playbook for automated server configuration.
- Install and configure Nginx automatically.
- Deploy a web application using an Ansible Jinja2 template.
- Demonstrate Ansible idempotency.
- Verify successful application deployment.

---

## 4. DevOps Lifecycle

The proposed DevOps lifecycle consists of the following stages:

1. Plan
2. Code
3. Build
4. Test
5. Release
6. Deploy
7. Monitor
8. Feedback

### Plan

Application requirements and deployment requirements are identified.

### Code

Application files and Ansible configuration are maintained using Git/GitHub.

### Build

A CI/CD pipeline can validate and build the application.

### Test

Syntax checks and application tests are performed before deployment.

### Release

The validated application is prepared for deployment.

### Deploy

Ansible automates server configuration and application deployment.

### Monitor

Application and server status can be monitored using logs and system
monitoring tools.

### Feedback

Monitoring results and user feedback are used for continuous improvement.

---

## 5. Proposed DevOps Architecture

The proposed architecture consists of:

Developer → GitHub → CI/CD Pipeline → Build & Test → Ansible →
Ubuntu Server → Nginx → Web Application → End User

The complete architecture diagram is included in the project submission.

---

## 6. Implemented Architecture

For the practical implementation, Ansible is executed in an Ubuntu
environment running through WSL2.

The implemented workflow is:

Ansible Playbook
        ↓
Ansible Configuration Management
        ↓
Ubuntu / WSL2
        ↓
Nginx Web Server
        ↓
HTML Web Application
        ↓
HTTP Port 80
        ↓
Web Browser

---

## 7. Technologies Used

| Technology | Purpose |
|------------|---------|
| Ansible | Configuration management and automation |
| Ubuntu | Target operating environment |
| WSL2 | Local Linux environment |
| Nginx | Web server |
| HTML/CSS | Web application |
| Jinja2 | Dynamic application template |
| Git/GitHub | Version control and proposed CI/CD integration |
| GitHub Actions | Proposed CI/CD pipeline |

---

## 8. Project Structure

```text
devops-ansible-assignment/
│
├── ansible.cfg
├── inventory.ini
├── site.yml
│
├── group_vars/
│   └── webservers.yml
│
└── templates/
    └── index.html.j2
