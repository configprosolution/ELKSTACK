# Docker-ELK Stack

[![Elastic Stack version](https://img.shields.io/badge/Elastic%20Stack-8.17.2-00bfb3?style=flat&logo=elastic-stack)](https://www.elastic.co/blog/category/releases)

This repository provides a **Dockerized ELK (Elasticsearch, Logstash, Kibana) stack** for centralized logging, monitoring, and analysis. The stack is orchestrated using `docker-compose`.

## Features
- **Elasticsearch**: Centralized storage and indexing of logs
- **Logstash**: Log ingestion and transformation pipeline
- **Kibana**: Web UI for data visualization and log analysis
- **Secure authentication**: Predefined users and roles
- **Fully containerized**: Easy deployment with Docker

## Prerequisites
- Docker (latest version recommended)
- Docker Compose
- At least 4GB RAM allocated to Docker

## Installation & Setup
1. **Clone the Repository:**
   ```sh
   git clone https://github.com/your-repo/docker-elk.git
   cd docker-elk
   ```

2. **Update Environment Variables (Optional):**
   Modify the `.env` file to configure user passwords and settings.

3. **Start the Stack:**
   ```sh
   docker-compose up -d
   ```

4. **Verify Services:**
   - Elasticsearch: http://localhost:9200
   - Kibana: http://localhost:5601

5. **Stop the Stack:**
   ```sh
   docker-compose down
   ```

## Configuration
- The `docker-compose.yml` file orchestrates the stack.
- Modify `logstash.conf` for custom Logstash pipelines.
- Update Kibana settings in `kibana.yml`.

## Usage
- Access Kibana at `http://localhost:5601`.
- Use Logstash to ingest logs.
- Query logs via Elasticsearch API.

## License
This project is licensed under the [MIT License](LICENSE).


