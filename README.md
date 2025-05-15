---

# API Gateway

This is the central entry point to the microservices architecture. It routes and filters incoming requests to the appropriate backend services using Spring Cloud Gateway.

## 🧩 Features

- Routing to backend microservices
- Path rewriting and load balancing
- Centralized API entry point
- CORS, security, and logging capabilities

## 🚀 Technologies

- Java 17
- Spring Boot 3
- Spring Cloud Gateway

## 📦 Routes (Example)

| Route Path        | Forwarded To               |
|-------------------|----------------------------|
| `/exchange/**`    | `exchange-rate-service`    |
| `/wallet/**`      | `wallet-service`           |

## 🛠️ How to Run

### Docker

```bash
docker build -t api-gateway .
docker run -d -p 8081:8081 --name api-gateway api-gateway
