# Automated College Website Deployment Using CI/CD

## Project Overview
This project demonstrates automated deployment of a static college website using DevOps tools and practices.

The website is hosted on AWS EC2 using Docker and Nginx. GitHub Actions automatically builds and deploys the updated Docker image whenever code is pushed to the main branch.

## Technologies Used
- AWS EC2
- Ubuntu Linux
- Docker
- Docker Hub
- Git and GitHub
- GitHub Actions
- Nginx
- Prometheus
- Node Exporter
- YAML
- SSH

## Architecture

```mermaid
flowchart TD
    A[Developer] --> B[GitHub Repository]
    B --> C[GitHub Actions CI/CD]
    C --> D[Build Docker Image]
    D --> E[Docker Hub]
    E --> F[AWS EC2]
    F --> G[Docker Container]
    G --> H[Nginx]
    H --> I[College Website]
    F --> J[Node Exporter]
    J --> K[Prometheus]
    K -.-> L[Grafana - Currently Stopped]

