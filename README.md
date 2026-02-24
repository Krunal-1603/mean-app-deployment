Project Summary

This project demonstrates end-to-end deployment of a full-stack MEAN (MongoDB, Express, Angular, Node.js) application using Docker, GitHub Actions CI/CD, AWS EC2, and Nginx reverse proxy.

The objective was to containerize, automate, and deploy the application in a production-style environment.

Frontend: Angular

Backend: Node.js + Express

Database: MongoDB

Containerization: Docker & Docker Compose

CI/CD: GitHub Actions

Cloud: AWS EC2 (Ubuntu)

Reverse Proxy: Nginx

Containerization

Separate Dockerfiles for frontend and backend

MongoDB using official Docker image

Multi-container setup managed via Docker Compose

Only Nginx exposed publicly (port 80)

CI/CD Pipeline

GitHub Actions pipeline:

Triggered on push to main

Builds Docker images

Pushes images to Docker Hub

EC2 pulls latest images and restarts containers

Deployed on AWS EC2 (t2.micro)

Configured Security Group for HTTP (port 80)

Dockerfiles (frontend & backend)

docker-compose.yml

nginx.conf

GitHub Actions workflow

Deployment screenshots


Outcome

Fully containerized application

CI/CD automated

Production-style reverse proxy setup

Cloud deployment successful

Infrastructure available for live demo
