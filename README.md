# Go HTTP Server 🚀

This project is a simple yet robust HTTP server built in Go. It provides essential functionalities like health checks, error handling, and JSON response formatting. It's designed to be easily extensible and serves as a great starting point for building more complex web services. The server utilizes the `chi` router for efficient request handling and includes CORS middleware for secure cross-origin communication. It solves the problem of setting up a basic, well-structured Go web server with built-in error handling and readiness probes.

## 🌟 Key Features

- **Health Check Endpoint:**  A `/healthz` endpoint that returns a 200 OK status, allowing for easy monitoring and readiness checks.
- **Error Handling:**  Includes a generic error handler (`/err`) to simulate and manage error conditions gracefully.
- **JSON Response Formatting:**  Provides utility functions for consistent and standardized JSON responses, including error messages.
- **CORS Support:**  Configured with CORS middleware to handle cross-origin requests securely.
- **Environment Variable Configuration:** Loads configuration from `.env` files for flexible deployment.
- **Modular Design:**  Well-structured codebase with separate handlers and utility functions for easy maintenance and extension.

## 🛠️ Tech Stack

- **Backend:**
    - Go
- **Routing:**
    - `github.com/go-chi/chi`
- **CORS:**
    - `github.com/go-chi/cors`
- **Environment Variables:**
    - `github.com/joho/godotenv`
- **JSON Handling:**
    - `encoding/json`
- **HTTP:**
    - `net/http`
- **Logging:**
    - `log`

## 📦 Getting Started

### Prerequisites

- Go installed (version 1.16 or higher)
- Git

### Installation

1.  Clone the repository:

    ```bash
    git clone <repository_url>
    cd <repository_directory>
    ```

2.  Install dependencies:

    ```bash
    go mod download
    ```

3.  Create a `.env` file in the root directory and define the `PORT` environment variable:

    ```
    PORT=8080
    ```

### Running Locally

1.  Run the server:

    ```bash
    go run main.go
    ```

2.  Access the endpoints:

    - Health check: `http://localhost:8080/v1/healthz`
    - Error endpoint: `http://localhost:8080/v1/err`

## 📂 Project Structure

```
.
├── .env                  # Environment variables configuration
├── go.mod                # Go module definition
├── go.sum                # Go module checksums
├── handler_err.go        # Error handler endpoint
├── handler_readiness.go  # Readiness probe endpoint
├── json.go               # JSON response utility functions
├── main.go               # Main application entry point
└── README.md             # Project documentation
```

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1.  Fork the repository.
2.  Create a new branch for your feature or bug fix.
3.  Make your changes and commit them with descriptive messages.
4.  Push your changes to your fork.
5.  Submit a pull request.

## 💖 Thanks

Thank you for checking out this project! I hope it's helpful.
