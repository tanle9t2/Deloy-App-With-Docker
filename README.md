# Deploy App With Docker

This repository is designed as a learning resource for deploying a web server application using Docker. It covers key concepts such as running web servers, securing them with Nginx and SSL, and integrating monitoring with Grafana.

## Purpose

- Learn how to deploy a web server using Docker containers
- Set up Nginx as a reverse proxy with SSL termination
- Monitor application metrics with Grafana

## Features

- Docker-based deployment for simplicity and portability
- Nginx configuration with SSL support (self-signed or custom certificates)
- Example setup for monitoring with Grafana dashboards

## Prerequisites

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/) (optional, if used)
- Basic familiarity with web servers and Linux command line

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/tanle9t2/Deloy-App-With-Docker.git
   cd Deloy-App-With-Docker
   ```

2. **Build and run the Docker containers:**
   ```bash
   docker-compose up --build
   ```
   > This will start the web server, Nginx with SSL, and Grafana services (if included in `docker-compose.yml`).

3. **Access the services:**
   - Web server: [https://localhost](https://localhost)
   - Grafana: [http://localhost:3000](http://localhost:3000) (default login: admin/admin)

4. **Customizing SSL Certificates:**
   - Replace the default self-signed certificates in the `nginx/certs` directory with your own if needed.

## Project Structure

- `Dockerfile` – Instructions for building the app container
- `docker-compose.yml` – Orchestration of all services
- `nginx/` – Nginx configuration and SSL certificates
- `grafana/` – Grafana provisioning (if present)
- `src/` – Application source code

## Monitoring with Grafana

- Grafana is pre-configured to visualize application or server metrics.
- Add your data sources and import dashboards via the Grafana web UI.

## Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements or questions.

## License

This project is licensed under the MIT License.

---

**Learning goals:** Docker, Nginx (with SSL), and Grafana integration.
