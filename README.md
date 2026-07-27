# Dockerized Flask Application

## Objective

This project demonstrates how to containerize a simple Flask application using Docker.

## Project Structure

```
app.py
requirements.txt
Dockerfile
.dockerignore
README.md
```

## Build the Docker Image

```bash
docker build -t flask-docker-app .
```

## Verify the Image

```bash
docker images
```

## Run the Container

```bash
docker run -d -p 5000:5000 --name flask-container flask-docker-app
```

## Access the Application

Open:

```
http://localhost:5000
```

Expected Output:

```
Docker is Working Successfully!!
```

## Stop the Container

```bash
docker stop flask-container
```

## Remove the Container

```bash
docker rm flask-container
```

## Technologies Used

- Python 3.12
- Flask
- Docker

## Learning Outcomes

- Created a Dockerfile
- Used a lightweight base image (`python:3.12-slim`)
- Added a `.dockerignore` file to reduce build context
- Built and ran a Docker container
- Verified that the application served correctly on `localhost:5000`
