# Comm-Docker-Monitoring

## Overview

The `comm-docker-monitoring` package provides a containerized monitoring solution using Grafana, Prometheus, and cAdvisor. It is designed to monitor and visualize the performance of Docker containers running on your system. This package includes pre-configured dashboards and data sources for Grafana and Prometheus, simplifying the setup process.

---

## Features

- **Grafana**: Interactive dashboards with visualizations for container metrics.
- **Prometheus**: Data collection and querying for real-time monitoring.
- **cAdvisor**: Collects container metrics like CPU, memory, and network usage.
- **Pre-configured setup**: Includes ready-to-use configurations for Grafana dashboards and Prometheus data sources.

---

## Requirements

Before installing the package, ensure that the following are installed on your system:

- **Docker**: Container runtime for running services.
- **Docker Compose**: Used to orchestrate multiple services.

---

## Installation

To install the package, follow these steps:

1. Ensure you have the necessary dependencies:
   ```bash
   sudo pacman -S docker docker-compose

## Usage

### Accessing Metrics in Grafana

To view metrics collected by the monitoring system, follow these steps:

1. **Open Grafana**:
   - Navigate to the URL in your web browser:
     ```
     http://localhost:3000
     ```

2. **Log in to Grafana**:
   - Use the default credentials:
     - **Username**: `admin`
     - **Password**: `biglinux`
   - (You can change these credentials in the `compose-monitor.yml` file under the `GF_SECURITY_ADMIN_USER` and `GF_SECURITY_ADMIN_PASSWORD` environment variables.)

3. **Navigate to the Docker Monitoring Dashboard**:
   - Once logged in, go to the following sections:
     - **Home** > **Dashboards** > **Docker Monitoring** > **Cadvisor exporter**.

4. **Explore Metrics**:
   - View visualizations for:
     - **CPU Usage**
     - **Memory Usage**
     - **Network Traffic**
     - **Container Start Times**
   - These dashboards provide detailed insights into the performance of your Docker containers.

---

This section ensures you can effectively utilize Grafana for monitoring your Docker containers.
