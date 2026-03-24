# Portfolio Website with Docker Compose Monitoring Stack

A containerized portfolio website with Prometheus and Grafana monitoring, deployed on AWS EC2.

## About This Project

This project was built as a hands-on learning exercise to understand Docker containerization and AWS EC2 deployment. The goal was to go beyond just running containers locally and actually deploy a multi-container application to the cloud with real monitoring infrastructure.

## What's Inside

The repository contains a Docker Compose setup that runs four services: an Nginx web server serving my portfolio site, an Nginx Prometheus exporter that exposes metrics, Prometheus for collecting those metrics, and Grafana for visualization. All services communicate over a shared Docker network.

## Tech Stack

Nginx (Alpine), Docker & Docker Compose, Prometheus, Grafana, AWS EC2 (Ubuntu), GoDaddy DNS

## Quick Start

```bash
git clone https://github.com/Trixxx12/Portfolio_Website.git
cd Portfolio_Website
docker-compose up --build -d
```

Then access the website at `localhost:8080`, Prometheus at `localhost:9090`, and Grafana at `localhost:3000`.

## Live Demo

- Website: http://54.243.162.28:8080
- Prometheus: http://54.243.162.28:9090
- Grafana: http://54.243.162.28:3000

## What I Learned

Building this project taught me how Docker layer caching works and why `--no-cache` matters when configs aren't updating. I learned the difference between Docker Compose V1 and V2, and why AWS Elastic IPs are essential for production deployments. The troubleshooting process also gave me practical experience with DNS propagation and debugging network connectivity issues.

## Author

**Bien Louis V. Barbachano**  
GitHub: [@Trixxx12](https://github.com/Trixxx12)
