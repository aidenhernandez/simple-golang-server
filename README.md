# Go Learning Projects

A collection of simple Go programs for learning the basics of the Go programming language.

## Projects

### 1. Hello World
**Location:** `helloworld/main.go`

A basic "Hello World" program that demonstrates the fundamental structure of a Go application.

**Features:**
- Simple console output using `fmt.Println`

**Running:**
```bash
cd helloworld
go run main.go
```

### 2. Simple Web Server
**Location:** `simpleWebServer/main.go`

A concurrent web server that counts the number of requests it receives. This project demonstrates HTTP handling, concurrency, and mutex usage in Go.

**Features:**
- HTTP server running on port 8080
- Thread-safe request counter using `sync.Mutex`
- Request logging with method and path
- 404 handling for non-root paths

**Running:**
```bash
cd simpleWebServer
go run main.go
```

Then visit `http://localhost:8080` in your browser. Each request to the root path will increment and display the counter.

**Implementation Highlights:**
- Uses `net/http` package for HTTP server functionality
- Implements mutex locks to prevent race conditions when incrementing the counter
- Logs all incoming requests with method and URL path
- Returns 404 for any path other than `/`

## Requirements

- Go 1.x or higher

## Learning Objectives

These projects cover:
- Basic Go syntax and program structure
- Package imports and usage
- HTTP server creation
- Concurrency and thread safety with mutexes
- Request handling and routing
- Logging

## License

This is a personal learning repository.
