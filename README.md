simple RESTful API built with [Gin](https://github.com/gin-gonic/gin) in Go, designed to manage a collection of music albums.

## Setup

1. **Clone the repository**
    ```bash
    git clone https://github.com/TBadru/RESTful-API-With-Go.git
    cd RESTful-API-With-Go
    ```

2. **Install dependencies**
    ```bash
    go mod tidy
    ```

3. **Run the application/start the server**
    ```bash
    go run main.go
    ```
    The API will be available at http://localhost:8080.

4. **Make a GET request to the running web service**
    ```bash
    curl http://localhost:8080/albums \
    --header "Content-Type: application/json" \
    --request "GET"
    ```
    ** This should display all the album list

5. **Make a POST request to the running web service**
    ```bash
    curl http://localhost:8080/albums \
    --include \
    --header "Content-Type: application/json" \
    --request "POST" \
    --data '{"id": "4","title": "Love Deluxe","artist": "Sade","price": 49.99}'
    ```
    ** This should display the headers and JSON for the added album
