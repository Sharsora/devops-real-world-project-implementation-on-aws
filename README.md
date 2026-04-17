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

<img width="579" height="602" alt="image" src="https://github.com/user-attachments/assets/5b143c4f-04ec-40ff-b9f3-0b614b23f688" />


---

## Step-04: Architecture Diagram

<img width="1155" height="586" alt="image" src="https://github.com/user-attachments/assets/8aa75f27-1309-48b3-88bf-8ce0bd23ce35" />

---
