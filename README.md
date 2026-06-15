## Deployment Environment

This project was built and tested on an AWS EC2 instance running Ubuntu.

### Infrastructure Used

* AWS EC2 (Ubuntu)
* Docker Engine
* Git & GitHub
* Flask Application

### Deployment Steps

1. Launch EC2 instance
2. Install Docker
3. Clone the GitHub repository
4. Build Docker image
5. Run container
6. Access application through EC2 Public IP

```bash
git clone <repository-url>
cd simple-flask-docker-project

docker build -t flask-app .
docker run -d -p 80:80 --name flask-container flask-app
```

### Application URL

```text
http://<EC2-PUBLIC-IP>
```

## Screenshots

### AWS EC2 Instance

*Add screenshot of your running EC2 instance from AWS Console.*

### Docker Image Build

*Add screenshot showing successful `docker build -t flask-app .` command.*

### Running Container

*Add screenshot showing `docker ps` output.*

### Application Running on Browser

*Add screenshot showing the Flask application accessed through the EC2 Public IP.*
<img width="1919" height="1019" alt="Running on browser" src="https://github.com/user-attachments/assets/b4ac1b23-5abd-4eca-9136-7dfaa1878259" />


### GitHub Repository

*Add screenshot of the GitHub repository containing the project.*
