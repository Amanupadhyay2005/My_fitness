# My_fitness
# 🏋️ AI-Powered Fitness Application

A scalable fitness platform built with **Spring Boot Microservices**, featuring AI-powered recommendations, secure authentication, and event-driven communication.

## 🚀 Features

* User registration and fitness activity tracking
* AI-powered fitness recommendations
* JWT authentication with Keycloak
* Asynchronous communication using RabbitMQ
* Service discovery with Eureka
* Centralized configuration with Spring Cloud Config
* React frontend

## 🏗️ Architecture

The project combines **Microservices Architecture** and **Event-Driven Architecture**.

```text
                    React Frontend
                          │
                          ▼
                   API Gateway
                       :8080
                          │
          ┌───────────────┼───────────────┐
          ▼               ▼               ▼
    User Service    Activity Service   AI Service
       :8081             :8082            :8083
          │               │                │
          ▼               ▼                ▼
     PostgreSQL        MongoDB          MongoDB
                          │
                          ▼
                       RabbitMQ
                          │
                          ▼
                    AI Processing
```

### Supporting Components

```text
Eureka Server       → Service Discovery
Config Server       → Centralized Configuration
Keycloak + JWT      → Authentication & Authorization
RabbitMQ            → Event-Driven Communication
```

## 🛠️ Tech Stack

**Backend:** Java, Spring Boot, Spring Cloud, Spring Security
**Architecture:** Microservices, Event-Driven
**Databases:** PostgreSQL, MongoDB
**Messaging:** RabbitMQ
**Security:** Keycloak, JWT
**Frontend:** React, Vite, Material UI

## 📂 Services

| Service          | Responsibility            |
| ---------------- | ------------------------- |
| User Service     | User management           |
| Activity Service | Fitness activity tracking |
| AI Service       | AI-based recommendations  |
| API Gateway      | Routing & security        |
| Eureka           | Service discovery         |
| Config Server    | Centralized configuration |

## 🔑 Key Highlights

* **Microservices Architecture** for scalability and independent service deployment.
* **Event-Driven Architecture** using RabbitMQ for asynchronous service communication.
* **API Gateway + Eureka** for routing and dynamic service discovery.
* **Keycloak + JWT** for secure authentication and authorization.
