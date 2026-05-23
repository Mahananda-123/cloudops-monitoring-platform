# CloudOps Monitoring and Automation Platform

## Project Overview

CloudOps Monitoring and Automation Platform is a scalable DevOps infrastructure monitoring solution designed to monitor multiple cloud servers in real time using Prometheus, Grafana, Alertmanager, Docker, Jenkins, and AWS EC2.

The platform enables centralized monitoring, automated alert management, CI/CD pipeline integration, and real-time infrastructure visualization for cloud-based environments.

---

## Objectives

* Monitor multiple Linux servers in real time
* Automate infrastructure monitoring and alerting
* Visualize system metrics through dashboards
* Implement CI/CD automation using Jenkins
* Deploy monitoring services using Docker containers
* Improve cloud infrastructure reliability and observability

---

## Key Features

* Multi-server centralized monitoring
* Real-time CPU, RAM, Disk, and Network monitoring
* Prometheus-based metrics collection
* Grafana dashboards for visualization
* Alertmanager email alert notifications
* Dockerized monitoring stack
* Jenkins CI/CD pipeline integration
* AWS EC2 cloud deployment
* Infrastructure observability and automation

---

## Technologies Used

* AWS EC2
* Docker & Docker Compose
* Jenkins
* Prometheus
* Grafana
* Alertmanager
* Node Exporter
* Linux (Ubuntu)
* Git & GitHub

---

## System Architecture

```text
Target Linux Servers
        ↓
    Node Exporter
        ↓
     Prometheus
        ↓
   Alertmanager
        ↓
 Grafana Dashboard
        ↓
      Jenkins
```

---

## Folder Structure

```text
devops-monitoring-platform/
│
├── monitoring/
│   ├── prometheus.yml
│   ├── alerts.rules.yml
│   └── alertmanager.yml
│
├── docker/
│   └── docker-compose.yml
│
├── jenkins/
│   └── Jenkinsfile
│
├── ansible/
├── backend/
├── frontend/
├── screenshots/
└── README.md
```

---

## Setup Instructions

### Clone Repository

```bash
git clone https://github.com/Mahananda-123/cloudops-monitoring-platform.git
cd cloudops-monitoring-platform
```

---

### Start Monitoring Stack

```bash
docker compose -f docker/docker-compose.yml up -d
```

---

## Access Services

Grafana:
http://13.126.36.179:3000

Prometheus:
http://13.126.36.179:9090

Alertmanager:
http://13.126.36.179:9093

Jenkins:
http://15.207.217.2:8080
---

## Monitoring Components

### Prometheus

Collects metrics from multiple servers using Node Exporter.

### Grafana

Provides real-time dashboards and visualization for infrastructure metrics.

### Alertmanager

Handles alert routing and sends email notifications during server failures or threshold breaches.

### Jenkins

Automates CI/CD workflows and infrastructure deployment pipelines.

### Node Exporter

Exports Linux system metrics such as CPU, memory, disk, and network usage.

---

## Future Enhancements

* Kubernetes monitoring integration
* Slack and Telegram notifications
* Advanced CI/CD deployment pipelines
* Docker container monitoring
* React-based monitoring dashboard
* Auto-scaling infrastructure support
* Ansible-based automated provisioning
* One-click deployment automation

---

## Conclusion

CloudOps Monitoring and Automation Platform provides an efficient and scalable solution for cloud infrastructure monitoring and DevOps automation. By integrating Prometheus, Grafana, Alertmanager, Docker, Jenkins, and AWS EC2, the platform enables centralized monitoring, automated alerting, and improved infrastructure reliability for modern cloud environments.
