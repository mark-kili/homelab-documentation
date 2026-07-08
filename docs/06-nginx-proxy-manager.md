# Nginx Proxy Manager

## Overview

Nginx Proxy Manager (NPM) is responsible for routing incoming traffic from my domain to the correct Docker services running inside my home lab.

Before deploying NPM, I could only access services locally using IP addresses and port numbers. After configuring a reverse proxy, I was able to access services through custom subdomains with HTTPS, creating a much cleaner and more secure experience.

---

## Objective

The objectives of deploying Nginx Proxy Manager were to:

- Learn how reverse proxies work.
- Access services using domain names instead of IP addresses.
- Secure applications with SSL certificates.
- Centralize access to self-hosted services.
- Simplify the management of multiple web applications.

---

## Why I Chose Nginx Proxy Manager

As my home lab continued to grow, I realized that remembering different IP addresses and port numbers for every application quickly became inconvenient.

For example:

Instead of accessing a service like this:

http://192.168.x.x:9443

I wanted something cleaner like:

https://portainer.zangetsu.xyz

Nginx Proxy Manager provides a simple web interface for configuring reverse proxies without requiring me to manually edit Nginx configuration files.

This made it much easier to learn reverse proxy concepts while keeping my infrastructure organized.

---

## Installation

Nginx Proxy Manager was deployed using Docker Compose.

The deployment included:

- Persistent storage
- MariaDB database
- Automatic restart policies
- Docker networking

After installation I confirmed that:

- The dashboard was accessible.
- Proxy Hosts could be created.
- SSL certificates could be generated.
- Internal Docker services were reachable.

---

## How It Works

The request flow is:

Internet
↓

Cloudflare DNS
↓

Nginx Proxy Manager
↓

Docker Container
↓

Application

This allows multiple services to share the same public IP while remaining accessible through different subdomains.

---

## Current Usage

Nginx Proxy Manager currently routes traffic for services including:

- Immich
- Portainer
- Future self-hosted applications

As additional services are deployed, they are added as new Proxy Hosts.

---

## Challenges Encountered

Deploying a reverse proxy introduced several networking concepts that were new to me.

Some of the challenges included:

- Understanding reverse proxies.
- Learning how DNS records work.
- Configuring SSL certificates.
- Troubleshooting routing issues.
- Learning how Docker networking interacts with Nginx Proxy Manager.
- Understanding ports and internal container communication.

Working through these challenges greatly improved my understanding of networking and self-hosting.

---

## Lessons Learned

Before this project, reverse proxies seemed like a complicated networking concept.

Building my own environment helped me understand that a reverse proxy is essentially a traffic manager—it receives incoming requests and forwards them to the appropriate service.

I also learned that exposing applications securely involves more than simply opening ports. DNS configuration, SSL certificates, networking, and proper routing all work together to provide secure access.

---

## Personal Reflection

Configuring Nginx Proxy Manager was one of the moments where my home lab started to feel like a real production environment.

Accessing my own applications through custom subdomains made the infrastructure feel much more professional and significantly improved my understanding of modern web hosting.

---

## Next Steps

After configuring the reverse proxy, I integrated Cloudflare to manage my domain, DNS records, and secure external access to my home lab.
