# Immich

## Overview

Immich is my self-hosted photo and video management platform. It serves as a personal alternative to cloud-based photo storage services, allowing me to retain full ownership of my media while learning how to deploy and maintain a modern, containerized application.

Deploying Immich was one of the first real-world applications I hosted after building the core infrastructure of my home lab.

---

## Objective

The objectives of deploying Immich were to:

- Learn to deploy a multi-container application.
- Understand how applications interact with databases and persistent storage.
- Explore self-hosting as an alternative to cloud services.
- Gain experience managing application updates and backups.
- Host a service that could be used in everyday life.

---

## Why I Chose Immich

I wanted to host an application that solved a real problem rather than simply deploying software for practice.

Immich stood out because it is actively developed, feature-rich, and designed as a self-hosted alternative to commercial photo storage platforms.

Deploying Immich also gave me an opportunity to work with a more complex Docker Compose stack involving multiple containers, environment variables, persistent volumes, and a PostgreSQL database.

Unlike many smaller applications, Immich represents the type of modern service commonly deployed in production environments, making it an excellent learning experience.

---

## Architecture

Immich consists of multiple services working together, including:

- Immich Server
- PostgreSQL Database
- Redis
- Machine Learning Service

Each service runs in its own Docker container and communicates over Docker networks.

This architecture introduced me to how modern applications are composed of multiple interconnected services rather than a single executable.

---

## Current Usage

Immich is currently used to:

- Store personal photographs.
- Upload videos.
- Organize media into albums.
- Access media through a web browser.
- Experiment with self-hosted cloud services.

---

## Challenges Encountered

Deploying Immich introduced several new concepts.

Some of the challenges included:

- Configuring Docker Compose correctly.
- Managing persistent storage.
- Understanding environment variables.
- Connecting PostgreSQL to the application.
- Troubleshooting container startup issues.
- Learning how multiple containers communicate with each other.

These experiences significantly improved my understanding of containerized applications.

---

## Lessons Learned

Immich taught me that modern applications are rarely made up of a single component.

Instead, they often depend on multiple services working together, such as databases, caching systems, storage, and background workers.

Deploying and maintaining Immich helped me become more comfortable reading documentation, understanding Docker Compose files, and troubleshooting interactions between containers.

It also reinforced the importance of planning storage, backups, and updates for applications that manage important personal data.

---

## Personal Reflection

Immich was one of the first applications I deployed that I could use in my daily life.

Seeing a self-hosted application operate successfully on infrastructure I built myself gave me confidence to continue exploring larger and more complex projects.

It also demonstrated the practical value of self-hosting beyond simply learning new technologies.

---

## Next Steps

After successfully deploying Immich, I continued expanding the home lab by deploying PostgreSQL to support both self-hosted applications and my own software development projects.
