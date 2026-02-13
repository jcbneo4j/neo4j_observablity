# Neo4j Observability Repo

This repository provides tools and configurations for Neo4j observability using Prometheus, Grafana, and Docker Compose for easy local setup.

## Features

- Prometheus exporter for Neo4j metrics collection.
- Pre-built Grafana dashboards for demonstrating database monitoring.
- Docker Compose for one-command observability stack deployment.


## Prerequisites

- Docker and Docker Compose installed.
- Neo4j instance with metrics enabled (`dbms.metrics.enabled=true`).


## Quick Start

1. Clone the repo: `git clone https://github.com/jcbneo4j/neo4j_observablity.git`
2. Navigate to the directory and start the stack:

```
cd neo4j_observablity
docker-compose up -d
```

3. Access Grafana at `http://localhost:3000` (admin/admin).
4. Update `docker-compose.yml` or `prometheus.yml` with your Neo4j endpoint.

## Configuration

- Edit `docker-compose.yml` to adjust ports and volumes.
- Configure Prometheus scrape targets in `prometheus/prometheus.yml`.
- Import additional dashboards via Grafana UI.


## Usage

- Monitor Neo4j metrics like query latency, transaction rates, and store sizes.
- View dashboards at Grafana localhost:3000.
- Stop the stack: `docker-compose down`.


