# MediiQuick Backend

Spring Boot backend for MediiQuick pharmacy delivery app.

## Requirements

- Java 17+
- Maven
- MongoDB running on localhost:27017

## Run Locally

```bash
mvn clean install
mvn spring-boot:run
```

## Run with Docker

```bash
docker build -t mediiquick-backend .
docker run -p 8080:8080 mediiquick-backend
```

## APIs

- POST /api/auth/send-otp?phoneNumber=xxxx
- POST /api/auth/verify-otp?phoneNumber=xxx&otp=yyy
- POST /api/medicines
- GET /api/medicines
- POST /api/cart/add
- GET /api/cart/{userId}
