# Myapp_B

A Spring Boot REST API application with user management functionality.

## Features

- User registration with email validation
- User management endpoints
- MySQL database integration with JPA/Hibernate
- RESTful API endpoints

## Tech Stack

- Java 21
- Spring Boot 4.0.3
- Spring Data JPA
- MySQL Connector
- Maven

## Endpoints

- `GET /demo` - Health check endpoint
- `GET /users` - Get all users
- `POST /register` - Register a new user

## Database Configuration

The application uses MySQL database with the following configuration:
- URL: `jdbc:mysql://localhost:3306/demo`
- Username: `root`
- Password: `Saiteja@2712`

## Running the Application

1. Make sure MySQL is running and the `demo` database exists
2. Run the application using Maven:
   ```bash
   mvn spring-boot:run
   ```
3. The application will start on port 2712

## API Usage

### Register a new user
```bash
curl -X POST http://localhost:2712/register \
  -H "Content-Type: application/json" \
  -d '{"username":"testuser","email":"test@example.com","password":"password123"}'
```

### Get all users
```bash
curl http://localhost:2712/users
```
# Myapp_b
