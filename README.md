# Spring Boot REST API

A complete RESTful API implementation using Spring Boot with JWT authentication, role-based access control, and OpenAPI documentation.

## Features

- **CRUD Operations**: Full resource management capabilities
- **Security**: JWT token-based authentication system
- **Role-Based Access Control**: Different permission levels for users
- **API Documentation**: Integrated Swagger/OpenAPI documentation
- **Data Persistence**: JPA integration with H2 database

## Technologies

- Java 11
- Spring Boot 2.5.4
- Spring Security
- Spring Data JPA
- JWT (JSON Web Tokens)
- H2 Database
- Swagger/OpenAPI

## Getting Started

### Prerequisites

- JDK 11 or higher
- Maven 3.6+ or Gradle
- Git

### Installation

1. Clone the repository
```bash
git clone https://github.com/Srini2005-Pro/Rest_API-Java.git
cd Rest_API-Java
```

2. Build the project
```bash
mvn clean install
```

3. Run the application
```bash
mvn spring-boot:run
```

The API will be available at `http://localhost:8080`

## API Documentation

Once the application is running, access the Swagger UI at:
```
http://localhost:8080/swagger-ui.html
```

## Authentication

The API uses JWT for authentication:

1. Obtain a token by sending credentials to `/api/auth/login`
2. Include the token in subsequent requests as a Bearer token in the Authorization header:
```
Authorization: Bearer {your_token_here}
```

## Project Structure

```
src/main/java/com/example/api/
├── config           # Configuration classes
├── controller       # REST controllers
├── dto              # Data Transfer Objects
├── entity           # JPA entity classes
├── repository       # Spring Data repositories
├── security         # Security and JWT classes
└── service          # Business logic services
```

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request
