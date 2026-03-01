# Application Config

Centralized configuration repository for microservices, containing environment-specific application properties for Spring Boot services.

## Configuration Files

| File | Purpose |
|------|---------|
| `application.properties` | Default/shared configuration |
| `application-dev.properties` | Development environment settings |
| `application-prod.properties` | Production environment settings |
| `application-jobms.properties` | Job microservice configuration |

## Tech Stack

- Spring Boot externalized configuration
- Spring Cloud Config compatible

## Usage

Reference this repository from a Spring Cloud Config Server or copy properties to individual microservices.

```yaml
spring:
  cloud:
    config:
      server:
        git:
          uri: https://github.com/Yashwanth9394/application-config
```
