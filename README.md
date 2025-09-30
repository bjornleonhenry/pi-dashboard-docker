# pi-dashboard-docker

# Raspberry Pi Dashboard (Docker)

A comprehensive monitoring dashboard for Raspberry Pi devices, containerized with Docker for easy deployment and management.

## Description

A containerized monitoring solution for Raspberry Pi devices with real-time system metrics and control capabilities.

## Features

- **Client**
  - Server status
  - Server uptime
  - CPU usage
  - Memory usage
  - Disk usage
  - Open Ports
  - Running Processes
  - Available updates
- **Server** (Python [FastAPI](https://fastapi.tiangolo.com/))
  - API's for client dashboard
  - Websocket for real-time updates
- **PB** [Pocketbase](https://pocketbase.io)
  - Database for storing server data

## Getting Started

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd pi-dashboard-docker
```

2. Set up environment variables by copying the example files and updating them with your configuration

### Server

Copy `/app/server/.env.example` to `/app/server/.env` and fill in your values.

### Client

Copy `/app/client/.env.example` to `/app/client/.env` and fill in your values.

### Run docker container

```bash
docker compose up --build -d
```
