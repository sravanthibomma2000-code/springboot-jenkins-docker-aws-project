# Spring Boot CI/CD Pipeline with Jenkins, Docker, DockerHub & AWS EC2

## Project Overview

This project demonstrates a complete End-to-End CI/CD pipeline for deploying a Spring Boot application using Jenkins, Docker, DockerHub, GitHub, and AWS EC2.

The pipeline automates the entire software delivery process from source code checkout to deployment on AWS EC2.

---

## Architecture

GitHub → Jenkins → Maven Build → Docker Build → DockerHub Push → Docker Deployment → AWS EC2

---

## Technologies Used

- Java 21
- Spring Boot
- Maven
- Jenkins
- Docker
- DockerHub
- GitHub
- AWS EC2
- Ubuntu Linux

---

## Project Features

✔ Automated CI/CD Pipeline

✔ Source Code Management using GitHub

✔ Maven Build Automation

✔ Docker Image Creation

✔ DockerHub Integration

✔ AWS EC2 Deployment

✔ Continuous Delivery Workflow

✔ Jenkins Pipeline as Code (Jenkinsfile)

✔ Infrastructure Hosted on AWS Cloud

---

## CI/CD Pipeline Stages

### 1. Source Code Checkout

Jenkins pulls the latest source code from GitHub.

### 2. Maven Build

Application is compiled and packaged using Maven.

### 3. Spring Boot Packaging

Builds executable JAR file.

### 4. Docker Image Build

Creates Docker image using Dockerfile.

### 5. DockerHub Push

Pushes Docker image automatically to DockerHub repository.

### 6. Docker Deployment

Runs Docker container on AWS EC2.

### 7. Application Hosting

Application becomes accessible through AWS Public IP.

---

## Docker Commands Used

### Build Image

```bash
docker build -t petclinic:v3 .
```

### Run Container

```bash
docker run -d --name petclinic-app -p 8082:8080 petclinic:v3
```

### Check Running Containers

```bash
docker ps
```

### View Docker Images

```bash
docker images
```

---

## DockerHub Repository

```text
sravanthibomma2000/petclinic:v3
```

DockerHub Repository:

https://hub.docker.com/r/sravanthibomma2000/petclinic

---

## Jenkins Pipeline

The Jenkins pipeline automates:

- GitHub Source Code Checkout
- Maven Build
- Docker Image Build
- DockerHub Image Push
- Docker Container Deployment

---

## AWS EC2 Deployment

Application is deployed on Ubuntu EC2 instance using Docker containerization.

Exposed Port:

```text
8082
```

---

## Live Application

Application URL:

```text
http://YOUR_PUBLIC_IP:8082
```

Example:

```text
https://100.31.116.116:8082
```

---

## Repository Structure

```text
springboot-jenkins-docker-aws-project
│
├── src/
├── Dockerfile
├── Jenkinsfile
├── pom.xml
├── README.md
└── docker-compose.yml
```

---

## Screenshots

### GitHub Repository

Shows project source code and CI/CD configuration.

### Jenkins Build Success

Demonstrates successful pipeline execution.

### DockerHub Repository

Shows Docker image pushed successfully.

### Live Application

Shows Spring Boot application running on AWS EC2.

---

## Outcome

Successfully implemented a complete DevOps CI/CD workflow using:

- GitHub
- Jenkins
- Maven
- Docker
- DockerHub
- AWS EC2

This project demonstrates practical DevOps skills including Continuous Integration, Continuous Delivery, Containerization, Cloud Deployment, and Infrastructure Automation.

---

## Author

Sravanthi Bomma

DevOps Engineer | AWS Cloud Engineer

GitHub:
https://github.com/sravanthibomma2000-code

DockerHub:
https://hub.docker.com/u/sravanthibomma2000
