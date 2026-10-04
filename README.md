# 🚀 AXION Cloud Deployment Platform

> Azure Kubernetes Service based application deployment platform using Docker, Kubernetes and CI/CD.

---

## 📌 Project Overview

AXION is a containerized application platform deployed on **Microsoft Azure Kubernetes Service (AKS)**.

The project demonstrates an end-to-end cloud deployment workflow covering:

- ☁️ Microsoft Azure
- ☸️ Azure Kubernetes Service (AKS)
- 🐳 Docker
- 🚀 CI/CD
- 🌐 Kubernetes networking and Ingress
- 📊 Application monitoring
- 🗄️ PostgreSQL database integration

---

## 🏗️ Application Components

| Component | Purpose |
|---|---|
| `axion-ui` | Frontend application |
| `axion-data-simulator` | Generates application and telemetry data |
| `axion-ingestion-service` | Processes and ingests incoming data |
| `axion-telemetry-query-service` | Queries telemetry data |
| `axion-database-schema` | Database schema and SQL definitions |

---

## ☸️ Kubernetes Architecture

The application components are deployed as Kubernetes workloads on **Azure Kubernetes Service**.

```text
                    Internet
                       |
                       v
             Azure Application Gateway
                       |
                       v
                 Kubernetes
                   Ingress
                       |
          +------------+------------+
          |            |            |
          v            v            v
      axion-ui     ingestion    telemetry
          |            |            |
          +------------+------------+
                       |
                       v
                  PostgreSQL
```

---

## ☁️ Azure Services

The deployment uses Azure cloud services including:

![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![AKS](https://img.shields.io/badge/AKS-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Application Gateway](https://img.shields.io/badge/Application_Gateway-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)

---

## 🔄 Deployment Flow

```text
Developer
    |
    v
Git Repository
    |
    v
CI/CD Pipeline
    |
    v
Docker Image
    |
    v
Container Registry
    |
    v
Azure Kubernetes Service
    |
    v
Application Gateway / Ingress
    |
    v
Application
```

---

## 🛠️ Technology Stack

### ☁️ Cloud

- Microsoft Azure
- Azure Kubernetes Service
- Azure Application Gateway

### 🐳 Containers & Kubernetes

- Docker
- Kubernetes
- Kubernetes Ingress
- AKS

### 🗄️ Application & Database

- Python-based services
- PostgreSQL
- REST APIs

### 🚀 DevOps

- Git
- CI/CD
- Containerized deployments
- Infrastructure automation

---

## 🎯 Key DevOps Practices

- Containerized application deployment
- Kubernetes workload management
- Service-based application architecture
- Ingress-based traffic routing
- Container image management
- CI/CD automation
- Cloud-native deployment on Azure
- Application and infrastructure troubleshooting

---

## 📂 Repository Structure

```text
AXION-Deployment03Oct/
│
├── axion-data-simulator/
├── axion-database-schema/
├── axion-ingestion-service/
├── axion-telemetry-query-service/
└── axion-ui/
```

---

## 👨‍💻 Author

### Ashwani Kumar

**Senior Azure DevOps Engineer**

Azure | Terraform | Kubernetes | AKS | Docker | CI/CD | Ansible

🌐 https://ashwaniai.site/

---

⭐ Built as a practical Azure DevOps and Kubernetes deployment project.
