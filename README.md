# Spring Shop API

A RESTful API built with Spring Boot for managing products.

## Tech Stack

- Java 26
- Spring Boot 4.0.6
- Spring Data JPA
- Spring Security
- PostgreSQL
- Maven

## Features

- CRUD operations for products
- Input validation
- Exception handling with proper HTTP status codes
- Service layer architecture

## Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /products | Get all products |
| GET | /products/{id} | Get product by ID |
| POST | /products | Create a product |
| PUT | /products/{id} | Update a product |
| DELETE | /products/{id} | Delete a product |

## Setup

### Prerequisites
- Java 26
- PostgreSQL

### Configuration

Create `src/main/resources/application.properties`:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/shopapi
spring.datasource.username=postgres
spring.datasource.password=YOUR_PASSWORD
spring.jpa.hibernate.ddl-auto=update
```

### Run

```bash
./mvnw spring-boot:run
```

### Test

```bash
./mvnw test
```

## Example Request

```json
POST /products
{
    "name": "T-Shirt",
    "price": 19.99
}
```
