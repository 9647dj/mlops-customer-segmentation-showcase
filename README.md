# ML Deployment & Customer Segmentation Showcase (Anonymized)

## Overview

This repository is a public portfolio-safe showcase of a team-based machine learning deployment project. The original project extended a machine learning workflow into a more reproducible, maintainable, and deployable ML system using MLOps practices.

The project focused on customer segmentation using clustering techniques on an anonymized automotive-style dataset. The goal was not only to build machine learning models, but also to structure the full workflow in a way that supports reproducibility, testing, deployment, monitoring, and team collaboration.

This version is intentionally limited and anonymized for public display. Sensitive dataset details, schema names, internal identifiers, and proprietary project references have been removed.

---

## Project Objectives

The project was designed to demonstrate the following:

- end-to-end ML pipeline understanding
- modular project organization
- reproducible machine learning workflow
- versioned model deployment
- API-based model serving
- monitoring and observability concepts
- CI/CD workflow exposure
- cloud deployment experience

---

## Key Features

- Modular ML pipeline from preprocessing to deployment
- Customer segmentation using clustering models
- Versioned deployment structure for promoted models
- Flask API for serving predictions
- Docker-based containerization
- Cloud deployment concepts using Google Cloud Run
- Monitoring concepts using Prometheus and Grafana
- Experiment tracking and reproducibility workflow
- Automated testing and CI/CD concepts using GitHub Actions

---

## ML Lifecycle Coverage

This project supports multiple stages of the machine learning lifecycle:

### 1. Data Preparation
Raw input data is cleaned and standardized before modeling.

### 2. Feature Engineering
Relevant clustering features are created from the prepared dataset.

### 3. Model Training
Clustering models are trained for segmentation tasks.

### 4. Hyperparameter Tuning
Candidate model settings are compared to select stronger configurations.

### 5. Model Promotion and Versioning
Selected models are packaged into versioned deployment folders.

### 6. API Deployment
Promoted models are served through a Flask API.

### 7. Monitoring and Observability
System and API behavior can be monitored through standard monitoring tools.

### 8. Testing and Reliability
Core components and API behavior are validated through testing workflows.

---

## My Contribution

This was a team project, and my contribution focused mainly on the engineering and deployment side of the workflow.

My work included:

- setting up Docker for the project environment and containerized workflow
- setting up Grafana and Prometheus for monitoring and observability
- organizing the initial project structure, including required folders and supporting files
- contributing to logging and monitoring-related setup
- setting up drift-related components for model monitoring concepts
- supporting configuration setup for a cleaner and more reproducible workflow
- contributing to testing-related setup and reliability practices
- building a strong end-to-end understanding of how the Python pipeline works across preprocessing, training, deployment, and monitoring

I use this project in my portfolio as a team-based MLOps and deployment project, with my role centered on system setup, monitoring, project structure, and workflow understanding.

---

## Technologies Used

- Python
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

## How the Tools Supported the ML Lifecycle

### GitHub
Used for version control, collaboration, and change tracking across the team workflow.

### DVC
Used for data versioning and reproducibility of datasets and pipeline inputs.

### MLflow
Used for experiment tracking, model artifact handling, and comparison of runs.

### Flask
Used to expose trained models through API endpoints.

### Docker
Used to package the application, dependencies, and serving environment into portable containers.

### Google Cloud Run
Used to deploy the containerized API in a cloud environment.

### Prometheus and Grafana
Used to support monitoring and observability for API health, performance, and system behavior.

### GitHub Actions
Used to automate testing and deployment workflows.

### Pytest
Used to validate API behavior and core project components.

---

## Technical Decisions and Trade-offs

### Modular Pipeline Structure
The workflow was separated into multiple pipeline stages instead of being kept inside one notebook or script.

**Why this helped:**
- easier to maintain
- easier to debug
- better for team collaboration
- easier to rerun only one stage when needed

**Trade-off:**
- more project structure to manage

### Docker-Based Environment
The project used Docker to create a more reproducible environment for serving and deployment.

**Why this helped:**
- same environment across systems
- easier handoff between team members
- simpler deployment workflow
- closer to real production practice

**Trade-off:**
- more setup and debugging effort compared with local-only execution

### Monitoring Stack with Prometheus and Grafana
Monitoring tools were added to improve observability of the API and system behavior.

**Why this helped:**
- made the project more production-oriented
- improved visibility into service behavior
- introduced real monitoring concepts beyond basic model training

**Trade-off:**
- adds complexity compared with a simple student notebook project

### Versioned Model Deployment
Promoted models were organized into deployment versions rather than replacing one active model file.

**Why this helped:**
- supports clearer deployment workflow
- makes rollback easier
- allows cleaner comparison between deployed versions

**Trade-off:**
- requires more file and release management

### API-Based Model Serving
The system used an API-based serving approach rather than limiting results to notebooks.

**Why this helped:**
- easier to demonstrate to others
- closer to industry ML deployment practice
- supports external use of the model

**Trade-off:**
- adds testing, deployment, and maintenance requirements

### Testing and Reliability
Testing support was included to improve confidence in the system.

**Why this helped:**
- catches errors earlier
- makes team collaboration safer
- supports cleaner deployment workflow

**Trade-off:**
- requires extra setup and maintenance time

---

## Simplified Project Structure

```bash
.
├── config/
├── data/
├── models/
├── monitoring/
├── outputs/
├── src/
│   ├── app.py
│   ├── preprocess.py
│   ├── feature_engineering.py
│   ├── train.py
│   ├── tune.py
│   └── promote_models.py
├── tests/
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
└── README.md# mlops-customer-segmentation-showcase
Anonymized ML deployment and MLOps project showcasing end-to-end pipeline, Docker, monitoring, and deployment concepts.
