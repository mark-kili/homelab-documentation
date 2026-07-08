# Network Configuration

## Overview

This document describes how I configured networking for my home lab to enable reliable communication between devices on my local network and secure access to self-hosted services.

A properly configured network is essential for hosting applications, accessing the server remotely, and exposing selected services to the internet.

---

## Objective

The objectives of this stage were to:

- Connect the server to the home network.
- Configure a static IP address.
- Enable remote management.
- Prepare the network for reverse proxy configuration.
- Configure external access using Cloudflare.

---

## Home Network

The server is connected to my home network through my router and is assigned a static IP address to ensure that its address remains consistent even after reboots.

Using a static IP simplifies the management of Docker services, reverse proxy configuration, and DNS records.

---

## Hostname

To make the server easier to identify on my network, I configured a custom hostname.

Hostname:

cronos

Using a meaningful hostname makes server administration much easier, especially when managing multiple devices.

---

## Remote Management

Once networking was configured, I enabled SSH so that I could manage the server remotely without needing to connect a monitor or keyboard.

Remote administration allows me to:

- Install software
- Update services
- Manage Docker containers
- Troubleshoot issues
- Maintain the server from another computer

---

## Cloudflare Integration

To securely expose selected services outside my home network, I configured Cloudflare for DNS management.

Cloudflare provides:

- DNS management
- SSL/TLS support
- Domain management
- Secure external access

My personal domain is:

zangetsu.xyz

Cloudflare allows me to access selected self-hosted applications using custom subdomains instead of remembering IP addresses.

---

## Why I Used a Static IP

A static IP address is important because several services depend on a consistent address.

Benefits include:

- Stable Docker networking
- Reliable reverse proxy configuration
- Consistent SSH access
- Easier troubleshooting
- Simpler DNS management

---

## Challenges Encountered

Networking has been one of the biggest learning experiences throughout this project.

Some of the challenges I encountered include:

- Learning how local networking works.
- Understanding DNS.
- Configuring Cloudflare.
- Troubleshooting connectivity issues.
- Learning the relationship between routers, DNS, reverse proxies, and Docker.

Each challenge improved my understanding of how self-hosted infrastructure communicates across a network.

---

## Lessons Learned

Networking is one of the foundations of every home lab.

Before starting this project, concepts such as DNS records, reverse proxies, and static IP addresses were mostly theoretical to me. Building this home lab allowed me to understand these concepts through practical experience.

One of the biggest lessons I learned is that many application issues are actually networking issues. Taking time to understand how devices communicate has made troubleshooting much easier.

---

## Next Steps

With the network configured, I was ready to install Docker and begin deploying applications using containers.

## Network Evolution

As I continued improving my home lab, my network configuration evolved over time.

Some of the improvements included:

- Moving from dynamic addressing to a static IP.
- Configuring Cloudflare DNS for external access.
- Experimenting with Pi-hole as the network DNS server.
- Learning how Docker networking interacts with reverse proxies.
- Troubleshooting connectivity issues while expanding the environment.

Each change improved both the reliability of my home lab and my understanding of networking concepts.
