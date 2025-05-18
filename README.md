# Rest_API-Java
# Spring Boot REST API

This project is a basic CRUD API for resource management built with Spring Boot. It implements JWT authentication and role-based access control, and it is documented using Swagger/OpenAPI.

## Features

- **CRUD Operations**: Create, Read, Update, and Delete resources.
- **JWT Authentication**: Secure endpoints with JSON Web Tokens.
- **Role-Based Access Control**: Different access levels for users based on roles.
- **API Documentation**: Automatically generated documentation using Swagger/OpenAPI.

## Project Structure

```
spring-boot-rest-api
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com
│   │   │       └── example
│   │   │           └── api
│   │   │               ├── ApiApplication.java
│   │   │               ├── config
│   │   │               │   ├── SecurityConfig.java
│   │   │               │   └── SwaggerConfig.java
│   │   │               ├── controller
│   │   │               │   └── ResourceController.java
│   │   │               ├── dto
│   │   │               │   └── ResourceDto.java
│   │   │               ├── entity
│   │   │               │   ├── Resource.java
│   │   │               │   └── User.java
│   │   │               ├── repository
│   │   │               │   ├── ResourceRepository.java
│   │   │               │   └── UserRepository.java
│   │   │               ├── security
│   │   │               │   ├── JwtAuthenticationFilter.java
│   │   │               │   ├── JwtTokenProvider.java
│   │   │               │   └── UserPrincipal.java
│   │   │               └── service
│   │   │                   ├── ResourceService.java
│   │   │                   └── UserService.java
│   │   └── resources
│   │       ├── application.properties
│   │       ├── static
│   │       └── templates
│   └── test
│       └── java
│           └── com
│               └── example
│                   └── api
│                       └── ApiApplicationTests.java
├── .gitignore
├── README.md
└── pom.xml
```

## Setup Instructions

1. **Clone the Repository**:
   ```
   git clone <repository-url>
   cd <source folder>
   ```

2. **Build the Project**:
   ```
   mvn clean install
   ```

3. **Run the Application**:
   ```
   mvn spring-boot:run
   ```

4. **Access the API**:
   The API will be available at `http://localhost:8080`.

5. **API Documentation**:
   Access the Swagger UI at `http://localhost:8080/swagger-ui.html` to explore the API endpoints.

## Usage

- Use the provided endpoints to manage resources.
- Authenticate using JWT tokens for secured endpoints.
- Refer to the Swagger documentation for detailed API specifications.

## License

This project is licensed under the MIT License.
