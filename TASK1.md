# SimpleTimeService

A minimalist microservice that returns the current UTC timestamp and the requester's IP address.

## Features
- Lightweight Python Flask app
- Runs as a non-root user
- Dockerized for containerized deployments

## JSON Response Format
```json
{
  "timestamp": "2025-05-15T12:00:00Z",
  "ip": "192.168.1.100"
}

Technologies Used
Python 3
Flask
Docker

How to Run This Project
1. Clone the Repository

git clone https://github.com/shankar7773/simple-time-service.git
cd simple-time-service

2. Build the Docker Image

docker build -t simple-time-service .

3. Run the Container (as non-root)

docker run -d -p 5000:5000 --name time-service simple-time-service

4. Test the Application

curl http://localhost:5000

DockerHub (Public Image)

This image is available on DockerHub:

Link: https://hub.docker.com/r/shankar7773/simple-time-service

