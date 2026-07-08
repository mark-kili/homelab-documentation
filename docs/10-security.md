# Security

## Overview

Security is an important consideration throughout my home lab. Although this environment is primarily used for learning and personal development, I aim to follow security best practices wherever practical.

Rather than exposing every service to the internet, I carefully choose which applications are publicly accessible and continuously improve the security of the environment as I learn more.

---

## Objective

The objectives of securing my home lab were to:

- Protect the server from unauthorized access.
- Secure services exposed to the internet.
- Minimize unnecessary attack surfaces.
- Learn Linux server security best practices.
- Build security awareness while self-hosting applications.

---

## Why Security Matters

Running services from home means I am responsible for protecting my own infrastructure.

Unlike cloud providers that manage much of the underlying security, a self-hosted environment requires me to think about:

- Who can access my server.
- Which ports should be exposed.
- How traffic reaches my applications.
- How software is updated.
- How data is protected.

Learning these concepts has been an important part of building my home lab.

---

## Current Security Measures

The following practices are currently implemented:

### SSH

- Remote administration is performed using SSH.
- SSH keys are used for authentication with services such as GitHub.
- Passwords are kept secure and are not shared.

### Firewall

Ubuntu's Uncomplicated Firewall (UFW) is used to restrict unnecessary network access.

Only required services are allowed through the firewall.

### Docker Isolation

Applications are deployed inside Docker containers, providing an additional layer of isolation between services and the host operating system.

### HTTPS

Services exposed externally are secured using HTTPS through Nginx Proxy Manager and Cloudflare.

### Software Updates

The server and installed applications are updated regularly to receive security patches and bug fixes.

---

## Security Philosophy

As my home lab grows, I prefer to expose as few services as possible.

Whenever possible:

- Services remain accessible only on the local network.
- Public services are routed through Cloudflare and Nginx Proxy Manager.
- Only necessary ports are opened.

This approach reduces the overall attack surface of the server.

---

## Future Improvements

Security is an area I plan to continue improving.

Planned enhancements include:

- Watchtower for container updates.
- Fail2Ban for intrusion prevention.
- VPN-only administration.
- Automated backup verification.
- Security monitoring.
- Improved logging and auditing.

---

## Challenges Encountered

One of the biggest challenges has been understanding how different layers of security work together.

During this project I have learned about:

- Firewalls
- Reverse proxies
- SSL certificates
- DNS security
- Docker networking
- Access control

These concepts initially seemed independent, but building the home lab helped me understand how they work together to secure an environment.

---

## Lessons Learned

Security is not a feature that is added after everything else—it is something that should be considered throughout the design of a system.

This project has taught me to think carefully before exposing services, opening ports, or deploying applications.

Perhaps the biggest lesson is that convenience should never completely replace good security practices.

Building a secure environment is an ongoing process rather than a one-time task.

---

## Personal Reflection

The more I build my home lab, the more I appreciate the importance of security.

Every new service I deploy is an opportunity to learn not only how it works, but also how it should be protected.

Although my security practices will continue to evolve, this project has given me a much stronger understanding of the responsibility that comes with self-hosting.

---

## Next Steps

With the infrastructure secured, the next priority is developing a reliable backup strategy to protect both application data and configuration files.
