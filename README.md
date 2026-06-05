# Spring Boot CI/CD Pipeline with Jenkins, Docker, DockerHub & AWS EC2

## Project Overview

This project demonstrates an end-to-end CI/CD pipeline for deploying a Spring Boot application using Jenkins, Docker, DockerHub, GitHub, and AWS EC2.

## Architecture

GitHub → Jenkins → Maven Build → Docker Build → DockerHub Push → Docker Deployment → AWS EC2

## Technologies Used

* Java 21
* Spring Boot
* Maven
* Jenkins
* Docker
* DockerHub
* GitHub
* AWS EC2
* Ubuntu Linux

## CI/CD Pipeline Stages

1. Source Code Checkout from GitHub
2. Maven Build
3. Package Spring Boot Application
4. Docker Image Build
5. DockerHub Image Push
6. Docker Container Deployment
7. AWS EC2 Hosting

## Docker Commands Used

Build Image:

```bash
docker build -t petclinic:v2 .
```

Run Container:

```bash
docker run -d --name petclinic-app -p 8082:8080 petclinic:v2
```

Check Running Containers:

```bash
docker ps
```

## DockerHub Repository

sravanthibomma2000/petclinic:v3

## Live Application

Application URL: Available on AWS EC2 (Port 8082)

## Outcome

Successfully implemented a complete DevOps CI/CD workflow using GitHub, Jenkins, Docker, DockerHub, and AWS EC2.
