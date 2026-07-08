# Cloudflare

## Overview

Cloudflare plays an important role in my home lab by providing DNS management for my domain and enabling secure access to selected self-hosted services.

Using Cloudflare allows me to access applications through memorable domain names instead of local IP addresses while adding an additional layer of security and reliability.

---

## Objective

The objectives of integrating Cloudflare were to:

- Manage DNS records for my domain.
- Route traffic to self-hosted services.
- Provide secure external access.
- Simplify domain management.
- Learn how DNS works in a real-world environment.

---

## Why I Chose Cloudflare

As my home lab expanded, I wanted to make my services accessible using my own domain instead of remembering local IP addresses.

Cloudflare offered an easy way to manage DNS records while providing additional security features and SSL support.

Another reason for choosing Cloudflare was its excellent documentation and free plan, making it ideal for learning and experimenting with self-hosted infrastructure.

Using Cloudflare also introduced me to concepts such as DNS propagation, A records, CNAME records, and proxying internet traffic.

---

## Domain

**Domain Name**

zangetsu.xyz

The domain acts as the public entry point to my home lab.

---

## Current Usage

Cloudflare is currently used for:

- DNS Management
- Subdomain Management
- SSL/TLS
- Secure routing to self-hosted services

Examples include:

- portainer.zangetsu.xyz
- immich.zangetsu.xyz

Additional subdomains are created as new services are deployed.

---

## Challenges Encountered

Learning Cloudflare introduced several networking concepts that were initially unfamiliar.

Some of the challenges included:

- Understanding DNS propagation.
- Learning the purpose of DNS records.
- Troubleshooting incorrect DNS configurations.
- Connecting Cloudflare with Nginx Proxy Manager.
- Understanding how requests travel from the internet to my home server.

Each issue strengthened my understanding of networking and internet infrastructure.

---

## Lessons Learned

Cloudflare taught me that DNS is much more than simply connecting a domain name to an IP address.

I learned how DNS records, reverse proxies, SSL certificates, and web servers all work together to make applications securely accessible over the internet.

Perhaps the biggest lesson was understanding that when something doesn't work, the problem isn't always the application—it could be DNS, networking, SSL configuration, or reverse proxy settings.

Learning to troubleshoot each layer individually has been one of the most valuable skills I've developed while building this home lab.

---

## Personal Reflection

Before starting this project, DNS felt like a concept that existed somewhere in the background of the internet.

After configuring my own domain and routing traffic to self-hosted applications, I now have a much better understanding of how internet services are discovered and accessed.

Cloudflare transformed my home lab from a local server into something that could be accessed using my own domain.

---

## Next Steps

Once external access was configured, I began deploying applications that would make use of the infrastructure, starting with Immich for self-hosted photo management.
