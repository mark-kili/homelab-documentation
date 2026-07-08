# Operating System Installation and Initial Configuration

## Overview

This document describes how I prepared my server after repurposing my HP Victus laptop into a dedicated home lab.

The goal was to create a stable Linux environment capable of hosting containerized applications, supporting software development, and providing a platform for learning system administration and self-hosting technologies.

---

## Objective

The objectives of this stage were to:

- Install Ubuntu Server
- Configure the server for remote administration
- Update the operating system
- Install essential utilities
- Prepare the server for Docker
- Establish a stable foundation for future services

---

## Operating System

| Item | Value |
|------|-------|
| Distribution | Ubuntu Server |
| Purpose | Self-hosted Home Lab |
| Installation Type | Clean Installation |

---

## Why Ubuntu Server?

Before settling on Ubuntu Server, I initially built my home lab using Debian. My goal was to learn the fundamentals of Linux server administration, remote access, and self-hosting.

Although Debian provided a stable learning environment, I found that some packages and drivers were not as up to date as I wanted for my use case. As I continued experimenting with Docker, self-hosted services, and AI-related workloads, I preferred an operating system that offered newer packages, excellent hardware compatibility, and a large community for troubleshooting.

For those reasons, I migrated my home lab to Ubuntu Server.

Ubuntu Server has proven to be a better fit for my environment because it:

- Provides more up-to-date software packages.
- Has excellent hardware and driver support.
- Works seamlessly with Docker and other self-hosting tools.
- Has extensive documentation and a large community, making it easier to troubleshoot and learn.

Migrating from Debian to Ubuntu also taught me that choosing an operating system isn't about finding the "best" distribution—it's about selecting the one that best supports your goals and workflow.
---

## Initial Server Configuration

After installing Ubuntu Server, I performed the following configuration tasks:

- Updated all system packages
- Configured SSH for remote management
- Installed Git
- Installed Curl
- Configured the system hostname
- Enabled automatic security updates where appropriate
- Prepared the server for Docker installation

---

## Essential Commands

Update package lists

```bash
sudo apt update
```

Upgrade installed packages

```bash
sudo apt upgrade -y
```

Install Git

```bash
sudo apt install git -y
```

Install Curl

```bash
sudo apt install curl -y
```

Verify the operating system

```bash
lsb_release -a
```

Check system information

```bash
hostnamectl
```

---

## Verification

After completing the initial setup, I confirmed that:

- The operating system booted correctly.
- Internet connectivity was working.
- SSH access was available.
- Package repositories were reachable.
- System updates completed successfully.

---

## Challenges Encountered

Like many Linux installations, configuring the server required becoming familiar with the command line and understanding package management.

As I continued building the home lab, I learned the importance of documenting configuration changes so they could be reproduced if the system needed to be rebuilt.

---

## Lessons Learned

Preparing the operating system is one of the most important stages of building a server.

A stable and well-maintained operating system reduces future troubleshooting and provides a reliable foundation for every service that will later be deployed.

This stage also helped me become more comfortable with Linux administration, package management, remote access, and maintaining an always-on server environment.

---

## Next Steps

With the operating system configured, the next stage was setting up networking so the server could communicate reliably with other devices and host self-managed services.

## Previous Environment

Before using Ubuntu Server, this home lab was initially deployed on Debian.

The migration to Ubuntu Server was part of my learning journey and gave me experience with:

- Installing multiple Linux distributions.
- Comparing server operating systems.
- Migrating services between environments.
- Rebuilding infrastructure after changing operating systems.
