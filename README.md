# Docker Demo Application

> This code is based on the [Docker & Kubernetes: The Practical Guide](https://www.udemy.com/course/docker-kubernetes-the-practical-guide) course by Maximilian Schwarzmüller on Udemy.

This is a simple Node.js application containerized with Docker. This README will guide you through the process of cloning the repository and running the application using Docker.

## Prerequisites

Before you begin, make sure you have the following installed:
- [Git](https://git-scm.com/downloads)
- [Docker](https://www.docker.com/products/docker-desktop/)

## Getting Started

### 1. Clone the Repository

#### For Windows Users:
```powershell
# Open PowerShell or Command Prompt
git clone https://github.com/ahmedbellaaj10/minimal-docker-nodejs.git
cd first-demo-starting-setup
```

#### For Linux Users:
```bash
git clone https://github.com/ahmedbellaaj10/minimal-docker-nodejs.git
cd minimal-docker-nodejs
```

### 2. Building and Running the Docker Container

#### For Windows Users:
```powershell
# Build the Docker image
docker build -t docker-demo .

# Run the container
docker run -p 3000:3000 docker-demo
```

#### For Linux Users:
```bash
# Build the Docker image
docker build -t docker-demo .

# Run the container
docker run -p 3000:3000 docker-demo
```

### 3. Accessing the Application

Once the container is running, you can access the application by opening your web browser and navigating to:
```
http://localhost:3000
```

## Additional Docker Commands

Here are some useful Docker commands you might need:

```bash
# List running containers
docker ps

# Stop a running container
docker stop <container_id>

# Remove a container
docker rm <container_id>

# List Docker images
docker images

# Remove a Docker image
docker rmi docker-demo
```

## Troubleshooting

If you encounter any issues:

1. Make sure Docker is running on your system
2. Ensure port 3000 is not being used by another application
3. Check if you have the necessary permissions to run Docker commands
4. For Windows users, ensure Docker Desktop is running

## Support

If you need any help or have questions, please open an issue in the repository. 