# Assessment

## Requirements
- Terraform
- Kubernetes
- Docker

## Instructions
1. Clone this repository:
    ```
   git clone https://github.com/muhammedriaz/cspeed-assessment
    ```
2. Build node app image (optional)
   ```
   docker build -t muhammedriaz/cspeed-backend ./node
    ```
    OR

    pull the image from Docker Hub (optional)
    ```
   docker pull muhammedriaz/cspeed-backend:latest
    ```
3. Test the application in Docker
    ```
   docker compose up --build -d
    ```
4. Go to `http://localhost/todo` to check if the API is functional. API endpoint references are given at the bottom.

## API Endpoint reference
- `GET /todo` - Retrieves all todos
- `GET /todo/{id}` - Retrieves a single todo by `id`
- `POST /todo` - Create a new todo
- `PUT /todo/{id}` - Update a todo by `id`
- `DELETE /todo/{id}` - Delete a todo by `id`
