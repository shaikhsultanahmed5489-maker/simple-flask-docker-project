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

<img width="1919" height="923" alt="ec2" src="https://github.com/user-attachments/assets/541f7cbb-606a-46bd-bb25-b10ec2f96a7f" />

### Docker Image Build & Running Container

<img width="1853" height="882" alt="docker build   ps" src="https://github.com/user-attachments/assets/c48d83d2-2bc0-47fd-b354-64d37ae90099" />

### Application Running on Browser

<img width="1919" height="1019" alt="Running on browser" src="https://github.com/user-attachments/assets/b4ac1b23-5abd-4eca-9136-7dfaa1878259" />
