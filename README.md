# SpringBootTodoApp

A simple Todo application built with Spring Boot and Kotlin.

## Technologies

*   Kotlin
*   Spring Boot
*   Spring Data JPA
*   PostgreSQL
*   Gradle

## Prerequisites

*   JDK 17 or later
*   PostgreSQL database

## Configuration

The application uses the following environment variables for database configuration. You can set these in your environment or use a `.env` file if supported by your setup.

| Variable | Default | Description |
| :--- | :--- | :--- |
| `HOST` | `localhost` | Database host |
| `PORT` | `5432` | Database port |
| `DATABASE` | `test` | Database name |
| `USERNAME` | `postgres` | Database username |
| `PASSWORD` | `mypassword` | Database password |

## Running the Application

1.  Ensure your PostgreSQL database is running and accessible.
2.  Build and run the application using Gradle:

    ```bash
    ./gradlew bootRun
    ```

## API Endpoints

The application exposes a REST API at `/api/todos`.

*   `GET /api/todos`: Get all todos
*   `GET /api/todos/{id}`: Get a todo by ID
*   `POST /api/todos`: Create a new todo
*   `PUT /api/todos/{id}`: Update an existing todo
*   `DELETE /api/todos/{id}`: Delete a todo
