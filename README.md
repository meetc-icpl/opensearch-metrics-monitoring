# OpenSearch Monitoring Stack with Prometheus and Grafana

## Project Overview
This project sets up a robust monitoring solution for OpenSearch using Docker Compose, featuring:
- **OpenSearch Cluster**: Two-node configuration
- **Prometheus**: Metrics collection
- **Grafana**: Performance visualization and dashboarding

---

## Prerequisites
- **Docker**
- **Docker Compose**
- **Minimum System Requirements**:
  - 2 CPU cores
  - 4GB RAM
  - 20GB disk space

---

## Architecture
The monitoring stack consists of:
- 2 **OpenSearch nodes**
- **OpenSearch Dashboards**
- **Prometheus**
- **Grafana**

---

## Installation Steps

### 1. Clone the Repository
    ```bash
    git clone <your-repository-url>
    cd <project-directory>

### 2. Configure Environment

    Modify docker-compose.yml to set custom passwords.
    Adjust memory and resource allocations as needed.

### 3. Start the Stack
    ```bash
    docker-compose up -d

---

### Access Points

    OpenSearch Dashboards: http://localhost:5601
    Prometheus: http://localhost:9090
    Grafana: http://localhost:3000

### Default Credentials

    Grafana:
        Username: admin
        Password: admin
    OpenSearch:
        Initial Admin Password: Set in docker-compose.yml

### Monitoring Configuration

## The setup automatically:

    Installs Prometheus Exporter for OpenSearch.
    Configures metric collection.
    Enables performance monitoring.

## Customization

    Modify Prometheus configuration in ./prometheus/prometheus.yml.
    Adjust Grafana dashboards as per your monitoring requirements.

### Troubleshooting

    Check container logs:
    ```bash
    docker-compose logs <service-name>

    Verify network connectivity.
    Ensure sufficient system resources.

Contributing

Contributions, issues, and feature requests are welcome!
Feel free to fork this repository and submit pull requests.
License

This project is licensed under the Apache 2.0 License.
