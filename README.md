# Uber-Like Application — Docker & CI/CD

A containerization project focused on building and running an Uber-like application using Docker and Docker Compose, with a development workflow managed through Git on Ubuntu.

## Overview

This project demonstrates how to containerize an existing Uber-like application and manage its services and dependencies using Docker-based tools.

The application is configured through Docker-related configuration files, allowing its required components to be built and started in a consistent environment. The project was developed and managed in an Ubuntu environment, with Git used for version control and GitHub for repository hosting.

The repository also serves as a foundation for implementing a CI/CD workflow to automate parts of the build and delivery process.

## Technologies Used

- **Docker** — Application containerization.
- **Docker Compose** — Service configuration and orchestration.
- **Ubuntu Linux** — Development and execution environment.
- **Git** — Version control.
- **GitHub** — Source code hosting and repository management.
- **CI/CD** — Continuous Integration and Continuous Delivery/Deployment workflow development.

## Project Structure

The repository includes the following Docker-related configuration files:

| File | Purpose |
|---|---|
| `Dockerfile` | Defines instructions for building a Docker image. |
| `docker-compose.yml` | Defines the application's services and their configuration. |

Other application components and dependencies are managed according to the existing project configuration.

## Getting Started

### Prerequisites

Before running the project, ensure that the following tools are installed:

- Docker Engine
- Docker Compose
- Git
- Ubuntu Linux or a compatible operating system

### Clone the Repository

```bash
git clone https://github.com/hamidili-code/uber-use-docker-extra-plus.git
cd uber-use-docker-extra-plus
```

### Build and Start the Application

From the directory containing the Compose configuration file, run:

```bash
docker compose up --build
```

This command builds the required images according to the available Docker configuration and starts the configured services.

To run the services in detached mode, use:

```bash
docker compose up --build -d
```

To stop the services, run:

```bash
docker compose down
```

**Note:** The actual startup process depends on the services, dependencies, environment variables, and configuration defined in the repository. Additional setup may be required.

## CI/CD Workflow

The project includes work with Git and an Ubuntu-based development environment and is intended to support CI/CD automation.

A CI/CD pipeline can be configured to automate tasks such as:

1. Checking out the source code from GitHub.
2. Building Docker images.
3. Running automated tests, when available.
4. Publishing images to a container registry, if configured.
5. Deploying the application to a target environment, if configured.

The steps above describe potential pipeline stages. Their implementation depends on the actual CI/CD configuration in the repository.

## Key Learning Objectives

- Understanding Docker-based application deployment.
- Building container images with a Dockerfile.
- Managing application services using Docker Compose.
- Working with Git and GitHub in an Ubuntu environment.
- Exploring the principles of CI/CD automation.

## Future Improvements

- Configure an automated CI/CD pipeline triggered by GitHub events.
- Add automated tests to validate application builds.
- Integrate a container registry for storing versioned Docker images.
- Document environment variables and service dependencies.
- Add deployment automation and application health checks.

## Author

**Hamidili**

GitHub: [@hamidili-code](https://github.com/hamidili-code)

---

*This repository focuses on Docker-based application setup and development workflow practices. Application-specific behavior depends on the underlying application code and configuration.*
