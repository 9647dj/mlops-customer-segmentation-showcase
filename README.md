# ML Deployment & Customer Segmentation (Anonymized)

## Overview

This project demonstrates an end-to-end machine learning deployment pipeline, transforming a prototype notebook workflow into a production-style system using MLOps practices.

The system performs customer segmentation using clustering techniques on an anonymized automotive-style dataset. The goal was to move beyond notebook-based experimentation and build a reproducible, scalable, and deployable ML workflow.

---

## Problem Statement

The project focuses on customer segmentation to support data-driven decision-making. The goal is to identify different customer behavior groups based on service and spending patterns.

A key challenge was converting a single notebook workflow into a structured system that supports:
- reproducibility
- modularity
- deployment
- monitoring
- scalability

---

## ML Pipeline Overview

The project follows a modular ML lifecycle:

1. Data preprocessing  
2. Feature engineering  
3. Model training (K-Means clustering)  
4. Hyperparameter tuning  
5. Model versioning and promotion  
6. API-based deployment  
7. Monitoring and observability  

---

## Model Summary

- Algorithm: K-Means Clustering  
- Scaling: Quantile Transformer  
- Evaluation Metrics:
  - Silhouette Score  
  - Calinski-Harabasz Score  
  - Davies-Bouldin Score  

Models were trained per segment group to capture different behavioral patterns and improve clustering quality.

---

## My Contribution

This was a team project. My contribution focused on the **engineering, deployment, and monitoring aspects** of the system.

Key contributions include:

- Designed and implemented **Docker-based containerization**
- Set up **Prometheus and Grafana** for monitoring and observability
- Implemented **logging and system monitoring workflows**
- Structured the **initial project architecture (folders, modules, configs)**
- Contributed to **drift and monitoring-related components**
- Worked on **configuration setup for reproducibility**
- Supported **testing and reliability workflows**
- Built a strong **end-to-end understanding of the ML pipeline in Python**

This project is presented as a **team-based MLOps system**, with my role centered on deployment, monitoring, and system structure.

---

## Technologies Used

- Python  
- Scikit-learn  
- GitHub  
- DVC  
- MLflow  
- Flask  
- Docker  
- Google Cloud Run  
- Prometheus  
- Grafana  
- GitHub Actions  
- Pytest  

---

## Deployment Architecture

### API Layer
- Flask REST API for predictions  
- Versioned endpoints (v1, v2)  
- Input validation and health checks  

### Containerization
- Docker used to package API and dependencies  
- Docker Compose used for multi-service setup  

### Cloud Deployment
- Deployed using Google Cloud Run  
- Auto-scaling serverless infrastructure  

---

## Monitoring & Observability

Monitoring was implemented using:

- Prometheus (metrics collection)
- Grafana (visual dashboards)

Tracked metrics include:
- API request rate  
- latency  
- errors  
- system resource usage  
- model-related metrics  

This enables real-time visibility into system performance.

---

## CI/CD & Testing

- GitHub Actions used for CI/CD pipelines  
- Automated testing for:
  - API endpoints  
  - health checks  
  - error handling  

This ensures stability and safe deployment of updates.

---

## Key Technical Decisions

### Modular Pipeline
Separated preprocessing, training, and deployment into modules  
→ improved maintainability and clarity  

### Docker-based Deployment
Ensured consistent environment across systems  
→ improved reproducibility  

### Monitoring Integration
Added Prometheus + Grafana  
→ improved visibility and system reliability  

### Versioned Models
Used version folders for deployment  
→ safer updates and rollback capability  

---

## Key Learnings

- Converting notebooks into production pipelines  
- Importance of reproducibility in ML systems  
- How containerization enables deployment  
- Role of monitoring in production ML  
- Differences between model development and deployment workflows  
- How team-based ML projects are structured in practice  

---

## Notes

- This is an anonymized version of a team project  
- Sensitive dataset details and internal identifiers have been removed  
- This repository focuses on demonstrating ML deployment concepts and workflow understanding  