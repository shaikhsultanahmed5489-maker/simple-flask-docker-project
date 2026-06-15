# Simple Flask Docker App

A basic Flask web application containerized using Docker.

This project was created to learn:

* Docker Images
* Docker Containers
* Dockerfile
* Docker Build Process
* Port Mapping
* Container Lifecycle Management

## Tech Stack

* Python 3
* Flask
* Docker

## Project Structure

```text
simple-flask-docker-app/
├── app.py
├── run.py
├── requirements.txt
├── templates/
│   └── index.html
└── Dockerfile
```

## Application Routes

| Route | Description |
| ----- | ----------- |
| /     | Home Page   |

## Run Without Docker

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
python run.py
```

Open:

```text
http://localhost:80
```

## Docker Commands

### Build Docker Image

```bash
docker build -t flask-app .
```

Verify image:

```bash
docker images
```

### Run Docker Container

```bash
docker run -d -p 80:80 --name flask-container flask-app
```

Verify container:

```bash
docker ps
```

Access application:

```text
http://localhost:80
```

### View Container Logs

```bash
docker logs flask-container
```

### Stop Container

```bash
docker stop flask-container
```

### Start Existing Container

```bash
docker start flask-container
```

### Restart Container

```bash
docker restart flask-container
```

### Remove Container

```bash
docker rm -f flask-container
```

### Remove Docker Image

```bash
docker rmi flask-app
```

## Learning Outcomes

Through this project, I learned:

* Creating Docker images using a Dockerfile
* Building images with `docker build`
* Running containers with `docker run`
* Mapping ports using `-p`
* Managing containers using Docker commands
* Viewing logs and troubleshooting containers
* Understanding the difference between images and containers

## Author

Sultan Ahmed Shaikh

Learning Docker and DevOps.
