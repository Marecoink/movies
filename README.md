# Movies Application

Welcome to the Movies Application! This Spring Boot application provides a backend for managing movies and reviews. It utilizes MongoDB for data storage. The frontend part was written with a little help from AI and tutorials :) 

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Setup](#setup)
- [Configuration](#configuration)
- [Endpoints](#endpoints)
- [Contributing](#contributing)
- [License](#license)

## Features

- Retrieve a list of all movies
- Get details of a single movie by IMDb ID
- Create reviews for movies

## Getting Started

### Prerequisites

Make sure you have the following installed:

- [Java](https://www.oracle.com/java/technologies/javase-downloads.html)
- [Maven](https://maven.apache.org/download.cgi)
- [MongoDB](https://www.mongodb.com/try/download/community)

### Setup

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/movies-application.git
    ```

2. **Navigate to the project directory:**

    ```bash
    cd movies-application
    ```

3. **Build the project:**

    ```bash
    mvn clean install
    ```

4. **Run the application:**

    ```bash
    mvn spring-boot:run
    ```

    The application will be accessible at [http://localhost:8080](http://localhost:8080).

## Configuration

You can configure the MongoDB connection in the `application.properties` file or by setting environment variables. See [Configuration](#configuration) for details.

## Endpoints

- **Get All Movies:**
  - **Endpoint:** `/api/v1/movies`
  - **Method:** `GET`

- **Get Single Movie:**
  - **Endpoint:** `/api/v1/movies/{imdbId}`
  - **Method:** `GET`

- **Create Review:**
  - **Endpoint:** `/api/v1/reviews`
  - **Method:** `POST`
  - **Request Payload:**

    ```json
    {
      "reviewBody": "A fantastic movie!",
      "imdbId": "tt1234567"
    }
    ```

## Contributing

Feel free to contribute to the project. Fork the repository, make your changes, and submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
