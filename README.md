# Spring Boot CI/CD Pipeline with Jenkins, Docker & AWS EC2

## Project Overview

This project demonstrates a complete CI/CD pipeline for deploying a Spring Boot application using Jenkins, Docker, GitHub, and AWS EC2.

## Architecture

GitHub → Jenkins → Maven Build → Docker Build → Docker Deployment → AWS EC2

## Technologies Used

* Java 21
* Spring Boot
* Maven
* Jenkins
* Docker
* GitHub
* AWS EC2
* Linux (Ubuntu)

## CI/CD Pipeline Stages

1. Source Code Checkout from GitHub
2. Maven Build
3. Package Spring Boot Application
4. Docker Image Build
5. Docker Container Deployment

## Docker Commands Used

Build Image:
docker build -t petclinic:v2 .

Run Container:
docker run -d --name petclinic-app -p 8082:8080 petclinic:v2

Check Running Containers:
docker ps

## Project URL

Application:
http://54.163.74.4:8082

## Jenkins Pipeline

The Jenkins pipeline automates:

* Source code checkout
* Maven build
* Docker image creation
* Application deployment

## AWS Deployment

The application is deployed on an AWS EC2 Ubuntu instance and exposed through port 8082.

## Outcome

Successfully implemented an end-to-end DevOps CI/CD workflow using Jenkins, Docker, GitHub, and AWS EC2.

