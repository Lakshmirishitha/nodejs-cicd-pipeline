# Node.js CI/CD Pipeline

## Description
This project demonstrates how to automate code deployment using GitHub Actions and Docker. A sample Node.js app is built and pushed to DockerHub using a CI/CD pipeline.

## What I Did
- Created a Node.js app using Express.
- Wrote a Dockerfile to containerize the app.
- Set up GitHub Actions in .github/workflows/main.yml to:
  - Install dependencies
  - Run test script
  - Build Docker image
  - Push to DockerHub
- Stored DockerHub credentials in GitHub Secrets (DOCKER_USERNAME, DOCKER_PASSWORD).

## DockerHub Repo
[View Image on DockerHub](https://hub.docker.com/r/jinka123/nodejs-demo-app)

## How to Run
```bash
docker pull jinka123/nodejs-demo-app
docker run -p 3000:3000 jinka123/nodejs-demo-app
