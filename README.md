## PostgreSQL Docker Compose Configuration

### Overview

This document explains how to use the Docker Compose file for setting up a PostgreSQL database, ideal for development purposes.

### Prerequisites

- Docker
- Docker Compose

### Configuration

- **Docker Compose Version**: `3.8`
- **Service**: PostgreSQL (`db`)
- **Image**: `postgres`

### Usage

1.  **Start the Database**:

    - Run `docker-compose up -d` in the directory with the `docker-compose.yml`.

2.  **Stop the Database**:

    - Use `docker-compose down` to stop the service.

### Details

- **Ports**: Maps host port `5432` to container port `5432`.
- **Environment**:
  - `POSTGRES_PASSWORD`: `password123` (Change for production)
  - `POSTGRES_DB`: `cartoon_db`
- **Volume**: `postgres-data` for data persistence at `/var/lib/postgresql/data`.
