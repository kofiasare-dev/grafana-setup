# Grafana, Tempo, Promtail, and Loki Stack

This repository contains a Docker Compose configuration for setting up a monitoring and logging stack using Grafana, Tempo, Promtail, and Loki.

## Prerequisites

Before getting started, make sure you have the following installed:

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Usage

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/your-repo.git
   cd your-repo
   ```

2. Customize configuration files:

You can customize configuration files for Grafana, Tempo, Promtail, and Loki by editing the corresponding files in the config directory.

3. Start the stack:

```bash
docker-compose up -d
```

4. Access Grafana:

Open your web browser and navigate to http://localhost:3000

## Services

### Grafana

Grafana is a powerful open-source platform for monitoring and observability. In this stack, Grafana is configured with anonymous authentication enabled and set to the "Admin" role for convenience.

Access Grafana at: http://localhost:3000

### Tempo

Tempo is a distributed, high-scale, and cost-effective tracing backend. It's used for collecting trace data.
Access Tempo at: http://localhost:8000

### Promtail

Promtail is an agent for collecting logs and sending them to Loki, which is the log aggregation system in this stack.

### Loki

Loki is a horizontally scalable, highly available, multi-tenant log aggregation system. It's used for storing and querying logs.

## Configuration

Configuration files for Grafana, Tempo, Promtail, and Loki are located in the config directory. You can modify these files to customize the

## Dependencies

This stack uses Docker Compose to manage the services, and it depends on the following images:

- Grafana: grafana/grafana:latest
- Tempo: grafana/tempo:latest
- Promtail: grafana/promtail:latest
- Loki: grafana/loki:2.9.0
