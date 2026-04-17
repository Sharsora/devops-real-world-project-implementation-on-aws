# Project: Retail Store Sample App

In this section, we’ll introduce the **Retail Store Sample App** — a real-world, cloud-native microservices application built and maintained by AWS Containers team. We’ll use this app.

---

## Step-01: What we’ll Learn

- Understand a real-world **microservices architecture**
- Explore how **multiple containers** work together as a system
- Set the stage for **Docker Compose**, **Kubernetes**, and **DevOps tooling**

---

## Step-02: Application Overview

This is a **10-container** app made up of:

- **5 Microservices**
  - Catalog (Go)
  - Cart (Java Spring Boot)
  - Checkout (NodeJS)
  - Orders (Java Spring Boot)
  - UI (Java Spring Boot)

- **3 Databases**
  - MySQL / MariaDB
  - PostgreSQL
  - DynamoDB Local (NoSQL)

- **1 Caching Server**
  - Redis

- **1 Messaging Server**
  - RabbitMQ

---

## Step-03: Component Diagram

> High-level view of services and their responsibilities

![Retail Store Component Diagram](../images/01-01-Retail-Store-Component-Diagram.png)

---

## Step-04: Architecture Diagram

> Shows how services connect, communicate, and depend on each other

![Retail Store Architecture Diagram](../images/01-02-Retail-store-Architecture-Diagram.png)

---
