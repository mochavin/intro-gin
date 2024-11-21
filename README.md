# Intro to Gin Web Framework

This repository provides a simple example of using the [Gin Web Framework](https://gin-gonic.com/) in Go. The example demonstrates how to build a basic CRUD API for managing an album collection. It serves as an introduction for beginners to understand the core concepts of Gin.

## Features

- Basic CRUD operations:
  - Create a new album
  - Retrieve all albums
  - Retrieve a single album by ID
- Uses JSON for data exchange

## Prerequisites

To use this project, you need the following:

- [Go](https://golang.org/dl/) (version 1.16 or later recommended)
- Basic understanding of Go language syntax and concepts
- Familiarity with RESTful APIs is helpful but not required

## Getting Started

1. **Clone the repository:**

   ```bash
   git clone https://github.com/mochavin/intro-gin.git
   cd intro-gin
   ```

2. **Install dependencies:**

   Run the following command to install required packages:
   ```bash
   go mod tidy
   ```

3. **Run the server:**

   Start the server using:
   ```bash
   go run main.go
   ```

   The server will run at `http://localhost:8080` by default.

4. **Test the endpoints:**

   Use tools like [Postman](https://www.postman.com/) or `curl` to interact with the API. Example endpoints:

   - `GET /albums`: Retrieve all albums
   - `GET /albums/:id`: Retrieve a specific album by ID
   - `POST /albums`: Add a new album

   Example `POST` request to add an album:
   ```json
   {
     "id": "3",
     "title": "New Album",
     "artist": "Artist Name",
     "price": 15.99
   }
   ```

## Project Structure

- `main.go`: Contains the main application code
- `go.mod`: Defines the Go module and dependencies

## Learning Goals

This project is designed to help you:

- Understand the basics of the Gin Web Framework
- Learn how to define routes and handle requests
- Familiarize yourself with JSON serialization and deserialization in Go
- Implement basic middleware for logging and error handling

## Resources

For further learning, check out these resources:

- [Gin Documentation](https://github.com/gin-gonic/gin)
- [Go by Example](https://gobyexample.com/)
- [Official Go Documentation](https://golang.org/doc/)
- [Web Service Gin](https://go.dev/doc/tutorial/web-service-gin)