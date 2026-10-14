# Dockerized Web Application — CodSoft DevOps Task 1

## Project Overview
A responsive web application containerized using Docker and served through Nginx. This project demonstrates containerization, web application deployment, and CI automation using GitHub Actions.

## Technologies Used
- HTML5
- CSS3
- Docker
- Nginx
- Git and GitHub
- GitHub Actions

## Features
- Responsive and modern web interface
- Lightweight Nginx web server
- Docker-based application deployment
- Automated Docker image build through GitHub Actions

## Run Locally

### 1. Build the Docker image
```bash
docker build -t codsoft-task-1 .
```

### 2. Run the container
```bash
docker run -d --name codsoft-web -p 8081:80 codsoft-task-1
```

### 3. Open the application
Visit http://localhost:8081 in your browser.

Port 8081 is used to avoid conflicts with other local services.

## CI Pipeline
The GitHub Actions workflow checks the required project files and builds the Docker image on pushes and pull requests targeting the main branch.

Workflow file: `.github/workflows/docker-ci.yml`

## Author
Harshita Singh

CodSoft DevOps Internship — Task 1
