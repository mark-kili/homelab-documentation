# PostgreSQL

## Overview

PostgreSQL is the primary relational database management system used throughout my home lab. It provides a reliable and scalable platform for storing application data while allowing me to develop, test, and manage my own software projects in an environment that closely resembles production.

Beyond supporting self-hosted services, PostgreSQL plays an important role in my software development workflow by acting as the backend database for several personal projects.

---

## Objective

The objectives of deploying PostgreSQL were to:

- Learn relational database administration.
- Host databases for personal software projects.
- Support containerized applications requiring persistent data.
- Gain hands-on experience with production-grade database systems.
- Build a development environment that mirrors real-world deployments.

---

## Why I Chose PostgreSQL

As I continued building applications, I realized that I needed a database system that was powerful, reliable, and widely used in the software industry.

After researching different database systems, I chose PostgreSQL because of its strong reputation, extensive feature set, and widespread adoption in modern web applications.

Another important reason was that many frameworks and applications I wanted to explore either recommend or officially support PostgreSQL.

Hosting my own PostgreSQL server also allows me to understand database administration beyond simply writing SQL queries. It gives me experience with installation, backups, networking, user management, and performance considerations.

---

## Installation

PostgreSQL was deployed as a Docker container within my home lab.

The deployment includes:

- Persistent storage for database files.
- Docker networking for secure communication.
- Environment variables for configuration.
- Automatic restart policies.

Running PostgreSQL inside Docker keeps the operating system clean while making deployments consistent and easy to reproduce.

---

## Configuration

The PostgreSQL server is configured to support multiple applications running within my home lab.

Configuration includes:

- Database creation.
- User and role management.
- Password authentication.
- Docker networking.
- Persistent data volumes.

Each application has its own database, allowing projects to remain isolated while sharing the same PostgreSQL server.

---

## Current Usage

PostgreSQL currently provides database services for:

- Personal software development.
- Backend API development.
- Future self-hosted applications.

As my projects continue to grow, additional databases will be created without requiring separate database servers.

---

## Real-World Applications

One of the main reasons I deployed PostgreSQL was to support software projects that I have personally developed.

### QuickPark

QuickPark is a digital parking lot booking and management system that I developed as part of my university project.

PostgreSQL stores:

- User accounts
- Parking slots
- Reservations
- Booking history
- Payment information

Using PostgreSQL allowed me to separate application logic from data storage while learning how modern web applications manage persistent data.

---

### MaliHub

MaliHub is a property management platform that I am currently developing.

The database is designed to manage:

- Organizations
- Property owners
- Caretakers
- Properties
- Housing units
- Tenants
- Lease agreements
- Rent payments
- Receipts
- Audit logs

Designing this database has helped me better understand database relationships, normalization, and scalable application design.

---

### Future Projects

As I continue building new applications, PostgreSQL will remain my primary relational database system.

Having a self-hosted database allows me to experiment, test new ideas, and deploy projects in a controlled environment without relying on external cloud database providers.

---

## Challenges Encountered

Working with PostgreSQL introduced me to many concepts beyond writing SQL.

Some of the challenges I encountered included:

- Understanding relational database design.
- Creating relationships between tables.
- Managing users and permissions.
- Connecting applications to the database.
- Configuring Docker networking.
- Protecting persistent data.

Each challenge improved my understanding of how databases support modern software systems.

---

## Lessons Learned

Deploying PostgreSQL taught me that a database is much more than a place to store information.

A well-designed database becomes the foundation of an application, influencing performance, scalability, and maintainability.

Building databases for my own projects also improved my understanding of:

- Database normalization.
- Primary and foreign keys.
- Data integrity.
- Backend application architecture.
- Real-world software design.

Perhaps the biggest lesson was realizing that good database design saves significant time later in the development process.

---

## Personal Reflection

PostgreSQL has become one of the most valuable services in my home lab because it directly supports the software I build.

Rather than relying on cloud-hosted databases for development, I now have complete control over my own database environment.

This has given me practical experience not only in application development but also in database administration, deployment, and maintenance.

---

## Next Steps

With the core infrastructure and database platform in place, the next stage of my home lab focuses on securing the environment, protecting data, and ensuring reliable operation through proper security practices and backup strategies.
