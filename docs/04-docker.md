# Docker

## Overview

Docker is the foundation of my home lab. Almost every service running on my server is deployed as a Docker container, making applications easier to install, manage, update, and remove.

Learning Docker has been one of the most valuable skills I've gained throughout this project. It introduced me to modern application deployment and helped me understand how production services are commonly managed.

---

## Objective

The objectives of this stage were to:

- Install Docker Engine
- Learn containerization
- Deploy applications using Docker Compose
- Isolate services from one another
- Simplify application management
- Build a scalable foundation for future services

---

## Why I Chose Docker

Before fully adopting Docker, I experimented with installing several services directly on the operating system. While this approach worked, I quickly realized that managing multiple applications became increasingly difficult.

Each service had its own installation process, configuration files, dependencies, and update procedures. Over time, the server became harder to organize and maintain because applications were scattered throughout the operating system.

Docker provided a much cleaner and more organized approach.

By running each application inside its own container, I was able to:

- Keep services isolated from one another.
- Reduce dependency conflicts.
- Standardize how applications are deployed.
- Make updates and maintenance much simpler.
- Easily remove and recreate services when needed.
- Keep the operating system clean and focused on running containers.

Another advantage I appreciated was the consistency Docker brought to my workflow. Almost every self-hosted application provides Docker installation instructions, making it much easier to deploy new services and keep my home lab organized.

After comparing both approaches, Docker became the obvious choice for managing my home lab, and it is now the foundation on which nearly all of my services run.

---

## Installation

Docker was installed on Ubuntu Server using the official Docker repository.

After installation, I verified that:

- Docker Engine was running.
- The Docker service started automatically after boot.
- Containers could be created successfully.

---

## Docker Compose

Docker Compose became the primary method for deploying applications.

Instead of running long Docker commands manually, I used compose files to define services, networks, volumes, and environment variables.

This approach makes deployments reproducible and easier to maintain.

---

## Services Running on Docker

At the time of writing, Docker is used to host:

- Portainer
- Nginx Proxy Manager
- Immich
- PostgreSQL

Additional services will continue to be added as the home lab grows.

---

## Directory Structure

To keep my server organized, I store Docker projects in dedicated directories.

Each application has its own folder containing:

- docker-compose.yml
- Environment variables
- Persistent volumes (where applicable)
- Configuration files

Keeping services separated makes maintenance much easier.

---

## Challenges Encountered

Learning Docker came with several challenges.

Some of the issues I encountered included:

- Understanding Docker images and containers.
- Learning how Docker volumes work.
- Managing Docker networks.
- Troubleshooting failed containers.
- Understanding bind mounts versus named volumes.
- Organizing compose files.
- Recovering services after configuration mistakes.

One memorable issue occurred after I renamed my home directory. Several Docker containers stopped working because their bind mount paths no longer existed. Troubleshooting and fixing this taught me how Docker references host directories and why consistent file paths are important.

---

## Lessons Learned

Before fully adopting Docker, I experimented with installing several services directly on the operating system. While this approach worked, I quickly realized that managing multiple applications became increasingly difficult.

Each service had its own installation process, configuration files, dependencies, and update procedures. Over time, the server became harder to organize and maintain because applications were scattered throughout the operating system.

Docker provided a much cleaner and more organized approach.

By running each application inside its own container, I was able to:

- Keep services isolated from one another.
- Reduce dependency conflicts.
- Standardize how applications are deployed.
- Make updates and maintenance much simpler.
- Easily remove and recreate services when needed.
- Keep the operating system clean and focused on running containers.

Another advantage I appreciated was the consistency Docker brought to my workflow. Almost every self-hosted application provides Docker installation instructions, making it much easier to deploy new services and keep my home lab organized.

After comparing both approaches, Docker became the obvious choice for managing my home lab, and it is now the foundation on which nearly all of my services run.

---

## Next Steps

After becoming comfortable with Docker, I wanted a better way to manage containers.

The next step was installing **Portainer**, which provides a graphical interface for managing Docker containers, images, networks, and volumes.
