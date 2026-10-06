# Movieist 🎬

Movieist is a Spring Boot REST API for managing movies and their reviews.

## Tech Stack

- Java 17
- Spring Boot
- Spring Web
- Spring Data MongoDB
- Maven
- MongoDB Atlas

## Project Structure

The application is organized into controllers, services, repositories, and model classes for movies and reviews.

```text
src/main/java/dev/sermo/movieist/
├── MovieistApplication.java
└── movies/
    ├── Movie.java
    ├── MovieController.java
    ├── MovieRepository.java
    ├── MovieService.java
    ├── Review.java
    ├── ReviewController.java
    ├── ReviewRepository.java
    └── ReviewService.java
```

## Requirements

- Java 17+
- Maven
- MongoDB / MongoDB Atlas

## Configuration

The application uses environment variables for MongoDB credentials:

```text
MONGO_DATABASE
MONGO_USER
MONGO_PASSWORD
MONGO_CLUSTER
```

MongoDB credentials should **never be committed to GitHub**.

## Running the Application

Start the application with:

```bash
mvn spring-boot:run
```

Or using the Maven wrapper:

```bash
./mvnw spring-boot:run
```

The application runs by default at:

```text
http://localhost:8080
```

## Testing

Run the tests with:

```bash
mvn test
```

## Building

Build the project with:

```bash
mvn clean package
```

## API

The REST API provides endpoints for movies and reviews.

The available routes are defined in:

- `MovieController`
- `ReviewController`

## License

This project is currently for educational and development purposes.
