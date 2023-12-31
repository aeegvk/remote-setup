# Remote Setup

This project is a multi-language development environment using Docker and Docker Compose.

## Directory Structure

- `.gitignore`: This file is used by Git to determine which files and directories to ignore when committing code.

- `README.md`: This file contains information about the project and instructions on how to use it.

- `code/`: This directory contains the source code for the project. It is divided into subdirectories for each programming language (Go, PHP, Python, Rust).

- `config/`: This directory contains configuration files for the project. The `env/` subdirectory contains environment-specific configurations.

- `data/`: This directory is used to store persistent data for the project, such as database files.

- `docker/`: This directory contains Docker-related files. Each subdirectory (`golang/`, `php/`, `python/`, `rust/`) contains a Dockerfile for building a Docker image for the corresponding programming language.

- `docker-compose.yml`: This file is used by Docker Compose to define and manage multi-container Docker applications. It specifies the services, networks, and volumes for the application.

- `scripts/`: This directory contains scripts for automating tasks in the project.

## Usage

To start the development environment, run the following command in the terminal:

```sh
docker compose up