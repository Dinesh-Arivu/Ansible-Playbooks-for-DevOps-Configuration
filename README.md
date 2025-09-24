# DevOps Automation Playbooks

This repository contains a collection of **Ansible playbooks** for automating common DevOps tasks, from web server setup to CI/CD pipelines, container management, and monitoring. Each playbook is modular and can be executed independently or combined for full-stack automation.

---

## 1. Web Server Installation (Nginx / Apache)
**Purpose:** Install and configure web servers.  
**Use Case:** Automate setup of web servers for applications.  
**Features:**
- Install Nginx or Apache
- Configure virtual hosts
- Deploy sample HTML pages
- Start and enable the web server service

---

## 2. Database Server Setup (MySQL / MariaDB)
**Purpose:** Install databases, secure them, and create DB/users.  
**Use Case:** Application database provisioning.  
**Features:**
- Install MySQL or MariaDB
- Remove anonymous users
- Set root password
- Create application database and user
- Configure permissions

---

## 3. Java / JDK Installation
**Purpose:** Install Java for Jenkins, Tomcat, or Java applications.  
**Use Case:** CI/CD pipeline prerequisites.  
**Features:**
- Install OpenJDK
- Configure JAVA_HOME
- Verify Java installation

---

## 4. Jenkins Installation & Job Configuration
**Purpose:** Setup Jenkins and create initial jobs.  
**Use Case:** Automate CI/CD pipelines.  
**Features:**
- Install Jenkins
- Start and enable service
- Configure admin user
- Create jobs via CLI or XML
- Install required plugins

---

## 5. Application Deployment (WAR / Docker / Static Files)
**Purpose:** Deploy web applications on Tomcat, Nginx, or Docker.  
**Use Case:** Automated artifact deployment.  
**Features:**
- Copy WAR or static files
- Pull Docker images
- Restart services or containers
- Manage ports and service availability

---

## 6. Docker Installation & Container Management
**Purpose:** Install Docker, pull images, and run containers.  
**Use Case:** Containerized application setup.  
**Features:**
- Install Docker
- Configure Docker group
- Create Docker networks
- Pull images and run containers with restart policies

---

## 7. ELK Stack Installation (Elasticsearch, Logstash, Kibana)
**Purpose:** Centralized logging and monitoring.  
**Use Case:** Log aggregation, dashboards, and alerts.  
**Features:**
- Install Elasticsearch, Logstash, and Kibana
- Configure services
- Set heap size, ports
- Configure restart handlers

---

## 8. CI/CD Pipeline Deployment
**Purpose:** Automate build, test, and deployment of applications.  
**Use Case:** Continuous integration & delivery.  
**Features:**
- Trigger builds
- Deploy artifacts
- Restart services
- Integrate with Jenkins, GitHub, or Docker

---

## 9. Monitoring & Alerting Setup (Prometheus / Grafana / Node Exporter)
**Purpose:** Infrastructure and application monitoring.  
**Use Case:** Collect metrics, create dashboards, send alerts.  
**Features:**
- Install Prometheus, Grafana, Node Exporter
- Configure scraping targets
- Create dashboards and alert rules

---

## 💡 Pro Tips for DevOps Playbooks
- **Use roles** to modularize playbooks (e.g., `roles/webserver`, `roles/db`, `roles/jenkins`).  
- **Store secrets securely** with Ansible Vault.  
- **Use idempotent tasks** to prevent repeated changes.  
- **Combine multiple playbooks** into a single pipeline for full-stack provisioning.

---

## License
This repository is licensed under the Apache License.  
