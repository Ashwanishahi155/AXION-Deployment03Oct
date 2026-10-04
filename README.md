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
| `axion-data-simulator` | Generates application/telemetry data |
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
       axion-ui    ingestion    telemetry
          |            |            |
          +------------+------------+
                       |
                       v
                  PostgreSQL
